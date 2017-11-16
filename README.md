# MNIST for ML Beginners using C#
  
This sample is a very simple WPF application which recognizes hand-written digits using the pre-built MNIST convolutional model. The MNIST problem is Machine Learning's Hello World program. 

MNIST is a simple computer vision dataset which consists of hand written digits like as shown below. 

<img src=https://msdnshared.blob.core.windows.net/media/2017/11/MNIST.png  alt="MNIST" />

This tutorial comes with a pre-built CNTK model which is trained to look at these hand-written digits and predict what these digits are. 

CNTK is a deep learning library in which this model is built in. For now, we will just basically load this model as a resource into your .NET application and evaluate on it.  Follow the steps below to get going. 

# Get Started 
1. If you are new to .NET, go ahead and download [Visual Studio 2017](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15) and select only the '.NET Desktop 

<img src=https://msdnshared.blob.core.windows.net/media/2017/11/dotnetdesktop.png alt="workload install" width="400" hieght="320"/>

2. Clone or [download](https://github.com/dotnet-architecture/MNISTTensorCNTK/archive/master.zip) this github repo. Open up the MNIST solution (MNIST.sln) file in Visual Studio 2017. 
                         
 <img src=https://msdnshared.blob.core.windows.net/media/2017/11/sln.png alt="workload install" width="800" hieght="270"/>

4.This solution consits of two projects 'Digitz' (C# project building a windows app using the CNTK pre-built MNIST model) and 
  'Training' (Python project, which generates the MNIST model using CNTK). Don't worry about the Python project for now. 
   
5. Set the start-up project to be 'Digitz' project as shown below and hit F5 (start) to launch the app.

The sample provides you an example of how you can use Tensor<T> today with CNTK for using a pre-built CNTK MNIST model. To use this sample just clone this repo and launch it in Visual Studio 2017.

[Tensor<T>](https://blogs.msdn.microsoft.com/dotnet/2017/11/15/introducing-tensor-for-machine-learning-and-ai-libraries) is an exchange type for homogenous multi-dimensional data for 1 to N dimensions. The motivation behind introducing Tensor<T> is to make it easy for Machine Learning library vendors like CNTK, Tensorflow, Caffe, Scikit-Learn to port their libraries over to .NET with minimal dependencies in place.  Tensor<T> is designed to provide the following characteristics.

<img src="https://msdnshared.blob.core.windows.net/media/2017/11/Tensor.png"     alt="Tensor<T> and CNTK"     style="float: left; margin-right: 10px;" />

To learn more about [Tensor<T> follow our blog post](https://blogs.msdn.microsoft.com/dotnet/2017/11/15/introducing-tensor-for-machine-learning-and-ai-libraries) and [GitHub repo](https://github.com/dotnet/corefxlab/tree/master/src/System.Numerics.Tensors). 
  
To follow a video tutorial on this app being used you can also follow this video. 
https://channel9.msdn.com/Events/Connect/2017/t126


  
  
  
  



