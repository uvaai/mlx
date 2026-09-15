## Deep Neural Networks and computational load

For this last machine learning module we'll complete the journey to modern deep neural networks, using _Tensorflow_ to define whole layers of the network, instead of writing a single Logistic regression unit by hand as in the first module. For this module we'll look at a few more interesting additions you can make to a neural network and practice using _Tensorflow_ to build the network.

As we arrive at more modern neural networks, we'll also quickly need a lot more computing power to optimize all the many weights that make up such a network. Running the assignments of this week on your own CPU is technically possible, but things will go much faster if you use a GPU (i.e. graphics card) to do the heavy lifting.

Having your code run on the GPU using Tensorflow is pretty straightforward, but does of course require that your computer has a good GPU (not standard and expensive). In addition, you'll need to separately install the GPU support for Tensorflow. If you have a good graphics card and would like to install this yourself, you can try this, but it is not recommended for this assignment. If you'd still like to try, instructions can be found here: https://www.tensorflow.org/install/gpu

## Running code online

The easiest way to run code on a GPU is probably by **Google Colab**. Colab offers (limited) computing resources completely for free for anyone with an account. Either service enables you to run your own Jupyter notebooks on quality GPUs without much hassle.

<!-- ## Running code online

The easiest way to run code on a GPU is probably by using **Kaggle** or **Google Colab**. Both offer (limited) computing resources completely for free for anyone with an account. Either service enables you to run your own Jupyter notebooks on quality GPUs without much hassle.

**We recommend you use Kaggle**, and only use Google Colab as an alternative for when Kaggle does not work. Kaggle has more transparent usage limits (30 hours of GPU usage per week) and can always offer you the same GPU, while Google Colab has dynamic usage limits that can throw you out at any time and does not always offer you the same hardware.

> Note that your GPU-time on either platform is limited. Try to remember to close the tab when you are working on other exercises or when you plan to go for lunch.

### Kaggle

Kaggle is a popular online platform and community for data science and machine learning enthusiasts funded and owned by Google. It serves as a hub for data-related challenges, boasting an extensive dataset repository, and, most importantly, offers a cloud-based Jupyter Notebook environment. To get started, create an account [here](https://www.kaggle.com/account/login?phase=startRegisterTab). *To be able to use a GPU in your online notebook, you will have to verify your account using your phone.* If you are uncomfortable doing this, we suggest you use Google Colab instead.

Upon logging in you will land on your dashboard. Verify your account using your phone. After verifying your account, find the a big plus sign in the menu on the left, where you can create a "New Notebook". This will open a standard notebook template. Disregard the contents of this template, go to "File -> Import Notebook" in the top left corner, and upload your `.ipynb` file. *Don't forget to change the notebook's name in the top left, so you can find it more easily in the future.*

Now all we have to do is to enable the GPU. Press the three vertical dots in the top right corner of the screen, and under "Accelerator" select "GPU P100". After confirming your choice, your notebook will now run on a GPU!

> If you want to access your notebooks after closing the tab, you can navigate to it using the menu on the left, selecting "Your Work". Your profile page will now be displayed. Press the "Code" tab on your profile and you will find your notebooks there!

##### A Convenient Kaggle feature

Kaggle offers a highly convenient feature; persistent storage of variables and files. This means that even after closing or disconnecting from a notebook, Kaggle will retain any created variables and downloaded files, saving time when you resume your work. _However, this feature is **not** enabled by default!_. Fortunately, enabling it is a straightforward process. When you've opened the desired notebook, access the "Notebook options" menu on the right. Within the "Persistence" section, choose "files only". With this selection, the persistence feature will be enabled, ensuring the preservation of your notebook's state across sessions. While you're there, change "Environment" to "Always use latest environment". -->

### Google Colab

A *Colab* is a Jupyter notebook that is not running on your own computer, but on one of Google's many cloud computers. In order to run this notebook as a Colab, go to https://colab.research.google.com/

On the Colab page, select *Upload*, upload your `.ipynb` file. Running a code cell on the Colab page will now actually run the code on a Google computer and not on your own machine!

Next we'll switch to a machine that has access to a GPU. In the menu at the top, select **Runtime** and then **Change runtime type**. Select the GPU hardware accelerator and Save. Now, any code you run will run on a Google GPU, which will make training your neural network much faster!

<!--
## Checking functionality

To check that everything works, run the code below in a cell:

    import tensorflow as tf

    print(tf.config.list_physical_devices('GPU'))


If everything is working correctly, you should see a single GPU listed as the device for your online notebook:

    [PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]

#### Kaggle: Could not resolve host?

It is possible that Kaggle gives an error in the cell that downloads the data; "could not resolve host". This can be solved with the following steps:    

1. Download the data file yourself from: https://www.cs.toronto.edu/%7Ekriz/cifar-10-python.tar.gz
2. In the sidebar under the Data section, there is a an icon to upload data, right next to big button to "Add Data". Upload the data file here and call it "cifar10".
3. Change the name of the folder in the cell below the download-cell from `'cifar-10-batches-py'` to `'/kaggle/input/cifar10/cifar-10-batches-py'`. **Note:** make sure you change the folder in both `unpickle`s!

You should now be able to skip the download cell, and continue the notebook as is.

#### Kaggle: Low accuracy on first cell?

Make sure you have "Environment" set to "Always use latest environment", and "Persistence" set to "files only". Restart your notebook by pressing the "Factory reset" button, or by stopping and re-opening the session. -->
