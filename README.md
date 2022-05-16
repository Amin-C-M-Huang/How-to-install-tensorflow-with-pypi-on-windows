# How-to-install-tensorflow-with-pypi-on-windows
The introduction on the market is generally to run tensorflow on jupyter, which requires the installation of many application suites (for example: cuda, numpy, scipy, cudnn, ....), the introduction here only needs to install the latest version of python that supports Tensorflow, you can run Tensorflow And Tensorflow-gpu, I hope it will help friends who want to try running machine learning on python, let's get started!


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
 
<h2>Step3. You need to install the numpy suite using pip.</h2>
<p>NumPy is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install numpy</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed numpy-1.22.3
</div></div>
    
<h2>Step4. You need to install the scipy suite using pip.</h2>
<p>SciPy is a free and open-source Python library used for scientific computing and technical computing.</p>
<p>SciPy contains modules for optimization, linear algebra, integration, interpolation, special functions, FFT, signal and image processing, ODE solvers and other tasks common in science and engineering.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install scipy</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed scipy-1.8.0
</div></div>
    
<h2>Step5. You need to install the graphviz suite using pip.</h2>
    <p>Graphviz is a package of open-source tools initiated by AT&T Labs Research for drawing graphs specified in DOT language scripts having the file name extension "gv". </p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install graphviz</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed graphviz-0.20
</div></div>    
    
<h2>Step6. You need to install the cuda suite using pip.</h2>
    <p>CUDA (or Compute Unified Device Architecture) is a parallel computing platform and application programming interface (API) that allows software to use certain types of graphics processing units (GPUs) for general purpose processing, an approach called general-purpose computing on GPUs (GPGPU). CUDA is a software layer that gives direct access to the GPU's virtual instruction set and parallel computational elements, for the execution of compute kernels. </p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install cuda-python</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed cuda-python-11.6.1 cython-0.29.28
</div></div>  
    
<h2>Step7. You need to install the cudnn suite using pip.</h2>
    <p>The NVIDIA CUDA Deep Neural Network library (cuDNN) is a GPU-accelerated library of primitives for deep neural networks. cuDNN provides highly tuned implementations for standard routines such as forward and backward convolution, pooling, normalization, and activation layers. </p>
You need to open your terminal/command prompt and enter the following commands:
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install nvidia-pyindex</div></div>
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>
	Successfully built nvidia-pyindex
	Installing collected packages: nvidia-pyindex
	Successfully installed nvidia-pyindex-1.0.9
</div></div>    
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install nvidia-cudnn</div></div>
You will get a success response, which means you have successfully installed.    
<h2>Step8. You need to install the Tensorflow suite using pip.</h2>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Tensorflow</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully built termcolor
Installing collected packages: tf-estimator-nightly, termcolor, tensorboard-plugin-wit, pyasn1, libclang, keras, flatbuffers, certifi, zipp, wrapt, werkzeug, urllib3, typing-extensions, tensorflow-io-gcs-filesystem, tensorboard-data-server, six, rsa, pyasn1-modules, protobuf, opt-einsum, oauthlib, idna, h5py, gast, charset-normalizer, cachetools, requests, keras-preprocessing, importlib-metadata, grpcio, google-pasta, google-auth, astunparse, absl-py, requests-oauthlib, markdown, google-auth-oauthlib, tensorboard, Tensorflow
Successfully installed Tensorflow-2.8.0 absl-py-1.0.0 astunparse-1.6.3 cachetools-5.0.0 certifi-2021.10.8 charset-normalizer-2.0.12 flatbuffers-2.0 gast-0.5.3 google-auth-2.6.6 google-auth-oauthlib-0.4.6 google-pasta-0.2.0 grpcio-1.46.0 h5py-3.6.0 idna-3.3 importlib-metadata-4.11.3 keras-2.8.0 keras-preprocessing-1.1.2 libclang-14.0.1 markdown-3.3.7 oauthlib-3.2.0 opt-einsum-3.3.0 protobuf-3.20.1 pyasn1-0.4.8 pyasn1-modules-0.2.8 requests-2.27.1 requests-oauthlib-1.3.1 rsa-4.8 six-1.16.0 tensorboard-2.8.0 tensorboard-data-server-0.6.1 tensorboard-plugin-wit-1.8.1 tensorflow-io-gcs-filesystem-0.25.0 termcolor-1.1.0 tf-estimator-nightly-2.8.0.dev2021122109 typing-extensions-4.2.0 urllib3-1.26.9 werkzeug-2.1.2 wrapt-1.14.1 zipp-3.8.0
</div></div> 

<h2>Step9. You need to install the Theano suite using pip.</h2>
<p>Theano is a Python library and optimizing compiler for manipulating and evaluating mathematical expressions, especially matrix-valued ones.[2] In Theano, computations are expressed using a NumPy-esque syntax and compiled to run efficiently on either CPU or GPU architectures.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Theano</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed theano-1.0.5
</div></div> 

<h2>Step10. You need to install the Tensorflow-gpu suite using pip.</h2>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Tensorflow-gpu</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed Tensorflow-gpu-2.8.0
</div></div> 

<h2>Step11.You can confirm if Keras is installed.</h2>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install Keras</div></div>
        
Your computer will tell you where your Keras is installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Looking in indexes: https://pypi.org/simple, https://pypi.ngc.nvidia.com
Requirement already satisfied: keras in c:\users\pmcn\appdata\local\programs\python\python39\lib\site-packages (2.8.0)
</div></div> 
    
<h2>Step12. You need to install the pandas suite using pip.</h2>
<p>pandas is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install pandas</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed pandas-1.4.2 python-dateutil-2.8.2 pytz-2022.1
</div></div> 
    
<h2>Step13. You need to install the Scikit-learn suite using pip.</h2>
<p>Scikit-learn (formerly scikits.learn and also known as sklearn)It features various classification, regression and clustering algorithms including support-vector machines, random forests, gradient boosting, k-means and DBSCAN, and is designed to interoperate with the Python numerical and scientific libraries NumPy and SciPy.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install -U scikit-learn</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed joblib-1.1.0 scikit-learn-1.0.2 threadpoolctl-3.1.0
</div></div> 
    
<h2>Step14. You need to install the matplotlib suite using pip.</h2>
<p>Matplotlib is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications using general-purpose GUI toolkits like Tkinter, wxPython, Qt, or GTK.</p>
You need to open your terminal/command prompt and enter the following commands:
    <div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>pip install -U Scikit-learn</div></div>
        
You will get a success response, which means you have successfully installed.
<div class="highlight-doscon notranslate"><div class="highlight"><pre id="codecell5"><span class="gp"></span>Successfully installed cycler-0.11.0 fonttools-4.33.3 kiwisolver-1.4.2 matplotlib-3.5.2 packaging-21.3 pillow-9.1.0 pyparsing-3.0.8
</div></div> 
<h3>Above, done!!</h3>


