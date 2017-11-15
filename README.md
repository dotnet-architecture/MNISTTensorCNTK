# MNIST Sample with Tensor<T> and CNTK
  
Tensor<T> is an exchange type for homogenous multi-dimensional data for 1 to N dimensions. The motivation behind introducing Tensor<T> is to make it easy for Machine Learning library vendors like CNTK, Tensorflow, Caffe, Scikit-Learn to port their libraries over to .NET with minimal dependencies in place.  Tensor<T> is designed to provide the following characteristics.
  
•	Good exchange type for multi-dimensional machine-learning data
•	Support for different sparse and dense layouts
•	Efficient interop with native Machine Learning Libraries using zero copies
•	Work with any type of memory (Unmanaged, Managed)
•	Allow for slicing and indexing Machine Learning data efficiently
•	Basic math and manipulation
•	Fits existing API patterns in the .NET framework like Vector<T>
•	Supports for .NET Framework, .NET Core, Mono, Xamarin & UWP
•	Doesn’t replace existing Math or Machine Learning libraries. Instead the goal is to give those libraries a sufficient exchange type for multi-dimensional data to avoid reimplementing, copying data, or depending on one another.

