# ENGR-E 534 Assignment 6: AI in Health and Medicine

# AI-enabled COVID-19 diagnostic framework utilizing Smartphone-based Embedded Sensors

Saptarshi Sinha, [fa20-523-312](https://github.com/cybertraining-dsc/fa20-523-312/), [Edit](https://github.com/cybertraining-dsc/fa20-523-312/blob/master/project/project.md)

**Keywords:** smartphone, neural networks, CNN, RNN, embedded sensors, symptom detection, cloud computing

## 1. Background: The need for smarter and more pervasive COVID-19 monitoring 

As mankind grapples with the menacing threat of an ongoing pandemic involving the novel COVID-19 (coronavirus infection), researchers and clinicians across the board have tirelessly involved themselves in myriad efforts for controlling the relentless proliferation of this virus so as to check the viral-driven casualties across the globe. It might seem that for the very first time, science and technology have been put to its greatest test ever. It seems that only time can tell if our scientific valor is indeed powerful enough to succeed in such a test, or if the virus would instead claim a major portion of the world’s population as its unfortunate casualty.

Numerous scientific approaches have been fielded in a relatively short amount of time to deal with the current problem. Many approaches involve novel technologies such as remote video surveillance using assistive robots that monitor virus-inflicted patients, while also protecting those healthcare workers by not involving them in such in-person diagnostic processes. Other approaches involve using machine learning based methodologies for sorting out patents with the virus from those without it simply by using an efficient algorithmic procedure of analyzing different aspects of patients’ CT scans. Major companies have also stepped in to assist in a war-footing format. As an example, Amazon Care is providing pick-up and delivery-based services of test-kits in particular virus-prone locations. Apple’s Siri is now able to provide symptom-based guidance in relation to COVID-19. Microsoft helped creating the Adaptive Biotechnologies platform that studies how our immune system responds to the virus which can provide insights for establishing drug development procedures. Finally, various biotechnological companies all across the world have started conducting extensive research into vaccine development and drug development procedures to combat this novel strain of the virus.        

As amazing these techniques might seem at a superficial glance, the major setback the world is suffering from is with the extent of the viral spread that is amplified due to the lack of testing capabilities. They are either inadequate or cannot handle an entire nation’s population. Although proactive actions have been employed in many nations, testing kits are still being produced slowly. This gives the virus an unfair advantage as time is of the essence. People (esp. asymptomatic individuals) with the virus remain undiagnosed for a greater length of time during which they can inadvertently aid with the proliferation of the viral disease. In this particular context, a very novel strategy for COVID-19 testing and diagnosis will be discussed that utilizes something that we all possess – a smartphone device.

## 2. Design & Working Principle: AI-based diagnostic framework for COVID-19 utilizing Smartphone-based Embedded Sensors and Artificial Neural Networks

Cornell University’s archive on Human Computer Interaction (HCI) features a recent article that discusses a strategy involving COVID-19 diagnosis with smartphone-based sensors. In its simplest form, the framework includes the smartphone, and its accompanying sensors and algorithms. External hardware accessories with high-power consumption, or access to specialized equipment is not required for this design [^1]. Since the application framework involves something that common people use on a daily basis, no tutorials or expert assistance is required to work with such an application. To understand the framework better, we must first note the various symptom types that are exhibited by COVID-19 patients which include high fever, tiredness, dry cough, intense headache, shortness of breath, nausea, etc. To efficiently capture the symptoms, an essential piece of information to keep in mind here is that modern smartphone devices come equipped with various in-built sensors viz. camera sensor, inertial sensor, temperature sensor, accelerometer sensor, microphones, etc. Many previous endeavors utilized such sensors to detect symptoms for other diseases [^1]. For instance, temperature-fingerprint sensor was used previously for measuring fever-levels; camera sensors (with accelerometers) were utilized earlier to analyze fatigue levels via pattern-recognition algorithms for human-gait analysis; camera sensor (with inertial sensor) were also used for analyzing neck posture to evaluate the headache severities; and, even the microphone was utilized previously for analyzing a patient’s cough-noise in a diagnostic process [^1].

The research article describes a strategy which uses these various smartphone sensors and their respective algorithms. This is followed up by creating a dataset record comprising predicted levels of the different symptoms which are collected from different patients and studied using deep learning approaches [^1]. Chiefly, it uses Convolutional Neural Networks (CNN) to analyze spatial data (viz. imaging data from the camera sensor), and Recurrent Neural Networks (RNN) for temporal data (viz. signal or text-based measurements) [^1]. The entire prediction-based framework can be summarized as follows:

![Smartphone-based framework for COVID-19 testing](images/Picture1.png)
<p>
    <img src="path_to_image" alt>
    <em>Figure 1: Smartphone-based framework for COVID-19 testing; Source: Adapted from [^1]</em>
</p>

The above framework can be sub-divided into four important layers which provides further insights into the different procedures going on in the background while the system makes the disease predictions.


### i. Reading 
The first layer involves reading based functionalities for the data coming from different smartphone sensors. This could refer to arrays of different types of data coming from different sources (viz. CT scan imageries, accelerometer readings, microphone sound signals, etc.).
### ii. Configurations 
The second layer deals with configuring onboard sensors for varied metrics such as time intervals, image resolution, etc. Readings from these first two steps are fed as inputs for the “symptoms algorithm” that can be executed as a smartphone application.
### iii. Symptoms Prediction 
The third layer deals with symptoms-level evaluation. The result is stored as a record that can be fed as an input for the next layer.  
### iv. COVID-19 Prediction
Finally, the last layer involves the application of deep learning (DL) based algorithms to the input data for predicting whether the patient has been afflicted with the virus. A CNN and RNN based combined process is utilized here such that the system can analyze both the spatial data (viz. image pixels) as well as the temporal data (viz. text/signal information) [1].

## 3. Discussions: Augmentation with Cloud-Comuputing capabilities 

To enhance the performance of this framework, the recorded data and predicted results can be uploaded to cloud-computing servers. This can help researchers and medical professionals from all around the globe in exchanging information and insights involving accurate patient diagnosis. Such applications are already developing. For instance, IBM recently launched the COVID-19 High Performance Computing Consortium [^2]. As the name suggests, this consortium has been explicitly designed to tackle the threat of COVID-19 by harnessing enormous computing power for streamlining the search for more information, aiding the hunt of possible treatment paths, and creating drug-and-disease based informational repositories that are made available to appropriate and eligible researchers and institutions strewn all across the globe [^2].    

All in all, it is indeed very commendable on the part of these researchers to facilitate the design of such a low-cost yet effective method of diagnosing COVID-19 when testing capacities are severely limited. If used appropriately, it can stem the spread of this virus by making it possible to diagnose patients sooner and quarantining them. Of course, the strategy does not focus on the treatment itself. But in the current scenario, where we have arrived at a breaking point with this disease, it would greatly assist healthcare personnel with locating and quarantining patients, that would indirectly help saving scores of other lives. 


## References:

[^1]: Maghdid, Halgurd S., et al. “A Novel AI-Enabled Framework to Diagnose Coronavirus COVID 19 Using Smartphone Embedded Sensors: Design Study.” ArXiv:2003.07434 [Cs, q-Bio], May 2020. arXiv.org, <http://arxiv.org/abs/2003.07434> </br> </br>
[^2]: D. Gil, “IBM Releases Novel AI-Powered Technologies to Help Health and Research Community Accelerate the Discovery of Medical Insights and Treatments for COVID-19”, ibm.com, Apr. 3, 2020. [Online]. Available: <https://www.ibm.com/blogs/research/2020/04/ai-powered-technologies-accelerate-discovery-covid-19/> [Accessed Oct. 17, 2020]
