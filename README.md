# How to install tensorflow with pypi on windows
The introduction on the market is generally to run tensorflow on jupyter, the introduction here only needs to install the latest version of python that supports Tensorflow, you can run Tensorflow-gpu, which requires the installation of many application suites (for example: cuda, numpy, scipy, cudnn, ....), I hope it will help friends who want to try running machine learning on python, let's get started!


<h2>Step1. You need to install python software.</h2>
    You need to go to the <a href="https://www.tensorflow.org/install">Tensorflow</a> official website to confirm the compatible version of Python. The following figure is an example to confirm that the compatible version of Python is 3.7–3.10. Here you can go to the official website of <a href="https://www.python.org/downloads/">Python</a> to download the highest compatible version. Here I downloaded Python 3.9.
    
<img width="1232" alt="截圖 2022-05-16 下午9 11 33" src="https://user-images.githubusercontent.com/97797926/168602516-e0d70f91-2554-4c29-9135-44b7bc89916d.png">

<h2>Step2. You need to install the pip suite.</h2>
<p>pip is the <a class="reference external" href="https://packaging.python.org/guides/tool-recommendations/">package installer for Python</a>. You can use it to install packages from the <a class="reference external" href="https://pypi.org/">Python Package Index</a> and other indexes.</p>
    There are 2 mechanisms to install pip supported directly by pip’s maintainers:
<section id="get-pip-py">
    <h3>
        <code class="docutils literal notranslate">
            <span class="pre">get-pip.py</span>
        </code>
        <a class="headerlink" href="#get-pip-py" title="Permalink to this headline"></a>
    </h3>
<p>This is a Python script that uses some bootstrapping logic to install pip.</p>
<ul>
    <li>
        <p>
            Download the script, from 
            <a class="reference external" href="https://bootstrap.pypa.io/get-pip.py">https://bootstrap.pypa.io/get-pip.py</a>.
        </p>
    </li>
    <li>
        <p>
            Open a terminal/command prompt, 
            <code class="docutils literal notranslate">
                <span class="pre">cd</span>
            </code>
            to the folder containing the
            <code class="docutils literal notranslate">
                <span class="pre">get-pip.py</span>
            </code> file and run:
        </p>
        <div class="tab-set docutils container">
        <input class="tab-input" id="tab-set--1-input--3" name="tab-set--1" type="radio"><label class="tab-label" for="tab-set--1-input--3"></label>
        <div class="tab-content docutils container">
        <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span> py get-pip.py</div></div>
</div>
<p></p>
</li>
</ul>
<p>More details about this script can be found in <a class="reference external" href="https://github.com/pypa/get-pip">pypa/get-pip</a>’s README.</p>
</section>
    You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed pip-22.0.4 wheel-0.37.1
</div></div>

<h2>Step3. Install the gpu environment.</h2>
The GPU environment requires two kits to be downloaded:
    <ul>
        <li>1. <a class="reference external" href="https://developer.nvidia.com/cuda-toolkit">CUDA</a></li>
        <li>2. <a class="reference external" href="https://developer.nvidia.com/cudnn">Cudnn</a></li>
    </ul>
Before downloading, you will need to go to the <a class="reference external" href="https://www.tensorflow.org/install/source_windows">Tensorflow</a> website to confirm the version.
    
<h2>Step4. You need to install the Tensorflow-gpu suite using pip.</h2>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Tensorflow-gpu</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed Tensorflow-gpu-2.8.0
</div></div> 


    

    

<h3>Above, done!!</h3>


