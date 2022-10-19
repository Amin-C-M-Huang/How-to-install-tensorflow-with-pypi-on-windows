# How to install tensorflow with pypi on windows
The introduction on the market is generally to run tensorflow on jupyter, the introduction here only needs to install the latest version of python that supports Tensorflow, you can run Tensorflow-gpu, which requires the installation of many application suites (for example: cuda, numpy, scipy, cudnn, ....), I hope it will help friends who want to try running machine learning on python, let's get started!


<h2>Step1. You need to install python software.</h2>
    Before downloading, you will need to go to the <a class="reference external" href="https://www.tensorflow.org/install/source_windows">Tensorflow</a> website to confirm the version.<br>
    
<img width="1232" alt="截圖 2022-05-16 下午9 11 33" src="https://user-images.githubusercontent.com/97797926/168602516-e0d70f91-2554-4c29-9135-44b7bc89916d.png">
Here you can see that the Python version supported by Tensorflow is 3.7-3.10.<br>
Let's download <a class="reference external" href="https://www.python.org/downloads/">Python version 3.8</a> in case some packages don't work.<br>
Pay attention to check Add Python 3.8 to PATH when installing. <br>
<img width="500" alt="python" src="https://user-images.githubusercontent.com/97797926/196619455-8cbfbdec-6b0a-44b5-896d-7c19288ee405.png">
The other steps will continue.<br>
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
    
<h2>Step3. Install the GPU kit.</h2>
The GPU environment requires two kits to be downloaded:<br>
    <ul>
        <li><a class="reference external" href="https://developer.nvidia.com/cuda-toolkit">CUDA</a></li>
        <li><a class="reference external" href="https://developer.nvidia.com/cudnn">Cudnn</a></li>
    </ul>
Before downloading, you will need to go to the <a class="reference external" href="https://www.tensorflow.org/install/source_windows">Tensorflow</a> website to confirm the version.<br>
    
<img width="1000" alt="tensorflow-gpu" src="https://user-images.githubusercontent.com/97797926/196614532-8f7387ba-c5e9-48ca-ba7e-6c65d53073e4.png">
For CUDA packages we install version 11.2.<br>
For the Cudnn package, we install version 8.1.<br>
After the cudnn package is downloaded, extract the files.<br>
Copy the extracted file to the following path:<br>
    C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2<br>
Replace the archive under the path.<br>
Next we need to add the path on the computer. <br>
Open PC settings->system->concerning->Advanced system settings->Advanced->environment variable->User variables->Path<br>
Then add the following environment variables:<br>
    <ul>
        <li>C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2\bin</li>
        <li>C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2\lib\x64</li>
        <li>C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2\libnvvp</li>
        <li>C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2\include</li>
    </ul>
Then you need to restart your computer.<br>
    
<h2>Step4. Install the Tensorflow-gpu suite using pip.</h2>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Tensorflow-gpu</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed Tensorflow-gpu-2.8.0
</div></div> 

Then you can start writing the program.<br><br>
If you want to make sure that you have installed it successfully, you can open the work administrator to confirm if the graphics card is working when running your program.    <br>

<h4>Other kits I have used:</h4>
    <ul>
        <li>pandas</li>
        <li>sdv</li>
        <li>matplotlib</li>
        <li>sklearn</li>
    </ul>
These can all be installed with pip.
<h3>Above, done!!</h3>


