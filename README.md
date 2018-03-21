# Machine learning on mobile


 Sound recognition today is a well-explored area. It is a favourite ML research topic and supported by big companies such as Google.  One of the modern challenges in this area is to make smart sound recognition available on mobile devices. The traditional architecture, when we gather raw data on the device, send it to the server that processes it and applies massive computations and then sends back the result, has its' downsides when is used on mobile: 
- sending raw data costs user time and money
- waiting for a result from the server can take a significant amount of time
- the service might not be available when the device is offline or has connection problems (being in remote locations)
- accumulated raw data increases expenses as it costs data storage and maintenance
-  keeping private data is a risk that has to  be approached and again costs money

We can change the architecture from a server-oriented to a client-oriented, that is sending a model to the device and applying it to the data there. It will solve these problems, but at the same time, it will reduce the number of the available models (that is not too heavy to use on a mobile). Also, it will diminish the learning side of it: once we used our "start-off" data, learned a model and send it to the device, we do not update the model anymore. 
The raw data gathered but the device is not included in the learning loop. To change this, we need to discover a mechanism that will allow mobile devices, once they have applied the model and got the result, to send this result back to the server where we can use it for updating the model. The new model then is distributed among all connected devices. 
The primary goals of this study are to investigate a possibility of a distributed learning with mobile devices and to experiment with real data by creating a simple mobile application. The possible data type is records of birds sounds with identifying tags.  Another possibility is to use images (for example of birds) with identifying tags.

Plan:
- make a list of models used in sound recognition 
- make a list of approaches used today in ML on mobile
- analyse these models for being used on mobile
- choose a model to apply 
- make an app architecture and design
- build app
- evaluate failure/success




    
