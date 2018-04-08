## Machine learning on mobile devices

It is almost impossible to imagine a life of a modern human without a smartphone. When machine learning becomes more and more embedded in digital world mobile devices cannot stand aside. Most of the ML techniques we've known so far require a lot of computational power. 
The only thing a mobile phone could do was to send a picture or a piece of text to a server with such computational power, where it would save this private data, process it and then send back some result. This approach has a few problems: private data collection with all its' complications and issues, connectivity and just lack of ability to work offline. 


Some hardware and software producers have already started to approach this problem. Lenovo announced a start of a creation of a new mobile device with processors designed for ML (http://news.lenovo.com/news-releases/lenovo-and-google-partner-on-new-project-tango-device.htm).  "Google Translate"  was adapted for mobile phones (https://research.googleblog.com/2015/07/how-google-translate-squeezes-deep.html). The app used a quite big convolutional neural net that could run on a superpowerful machine with no problem. It had to be reduced and restricted or "squeezed" to fit mobile devices abilities. All of the learning happened in the Google Labs. It took some time to make it usable with real world letters. As a result, they created a small net that any phone could use even offline.  


Not long time ago a new lite version of TensorFlow was introduced for Android and iOS https://www.tensorflow.org/mobile/tflite/). Now it is possible to run previously impossible ML algorithms on mobile hardware and without connecting to the cloud. 
According to the TensorFlow Lite architecture (https://www.tensorflow.org/images/tflite-architecture.jpg) a mobile device downloads a trained model and applies it to the data gathered by the device without "leaving" it. 

This approach solves two problems, data privacy and ability to work offline. Still, it has a few issues. 
It works only with some a limited number of types of models for now. There is a TensorFlow Mobile project for those whos model does not fit the Lite version constraints (https://www.tensorflow.org/mobile/mobile_intro). 
But a more critical downside of this approach is that we lose the power of distributed knowledge that we can use for further learning. Once we have learned a model and sent it to a mobile device, we don't change it. We could find a way to evaluate the model right on the device and send the feedback to the central server, where it can use this data from numerous phones to improve the model and distribute it among them back again. Keeping this cycle can help to continue the learning with the help of distributed leraners. 

Next steps: 

* take an existing bird songs recognition model and find out it fits either TensorFlow Lite or TensorFlow Mobile
* analyse the model for possible use in a distributed learning architecture

