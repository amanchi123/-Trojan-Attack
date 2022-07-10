#Assurance to Machine Learning Models:
Project Title: Advanced Algorithms for Machine Learning-P82

State-of-the-art Machine Learning methods are always black-box models, i.e., we do not know how the model behaves during the training and inference phases. In many real-world applications, the prediction accuracy is not the only factor when making decisions. Instead, should focus on fairness , explain ability of the model.
Developed a computational framework that is flexible to address various aspects of the assurance problems e.g., fairness, robustness, interpretability using Deep Learning (CNN) at its core.
Contents 
 Abstract 
 Introduction 
 Literature Review 
 Proposed Work 
 Experimental Results 
 Conclusion 
 Future Scope. 
Abstract: 
In the modern era, where whole universe relay on electronic connectivity, the 
percentage of hackers, electronic frauds got increased and creating hazardous 
effects to the society. There is indeed no time at which security does not matter. It is 
very important to ensure the need to protect the data and systems from network 
related attacks and to gain trust of firms and customers. In the recent years, fraud 
attacks became most common in the field of AI where the attacker try poisoning the 
pre trained data in other words masquerade the training data such attacks are 
known as Trojan attacks. Trojan attacks are commonly seen in Neural Network 
applications such as Voice Recognition, Self driving Vehicles, Machine Learning 
models, Robotics, Voice recognition apps etc. In this report we will discuss on the on 
the concepts of neural Trojan attacks, discussed on existing related work for 
Backdoors and its defense methods finding out the best suggest able method by 
surveying on different papers and implemented concept of Badnets considering the 
MNIST dataset in real time by building the clean model using CNN model with an 
model performance of about 98%. Creating Poisonous model with performance rate 
of 100% . Implementing defence technique STRIP to check for accuracy of the model 
and recover to original model with performance rate of 92%. 
Introduction: 
 DNN is widely used for face, image recognisation and in solving classification models. 
Building DNN model is very complex process so many business follow the two 
methods to perform the computations on Neural Networks by below methods: 
 
 1.Fully Sourced Training 
 2. Transfer Learning. 
 
 Literature Review: 
 From the past 3 years ,there took place many such attacks which demanded for the 
design proposal techniques for securing from these attacks.Initially backdoor attacks 
took place in Machine Learning models in the form of Exploratory and Causative 
attacks which involves malwaring of data during testing and training instance 
respectively. The attacker goal was to craft message but with the advanced of 
technology the security concerns started increasing as the attackers became smarter 
and attacks on DNN took place. 
 Related work deals with the training inputs of Deep Learning model being poisoned 
and model misbehaves with clean data. Later, came the advanced techniques where 
model behaves well with clean data and misbehaves as per attackers backdoor 
without disturbing the overall efficiency of the model. Below Fig-1 illustrates the in 
detail mechanism of the category of defense and attack strategies. 
Existing Badnet Models: 
 Considering real time examples to find the backdoor attacks in DNN 
using real time example of MNIST digitbuilt clean model using 3layered CNN model with two 
CNN layers with fully connected output layer. 
Backdoor attack is designed by randomly selecting 7 digit and activating the 
trigger to produce misclassification. Fig-1 illustrates pictorial presentation in detail.
Defense Techniques: 
STRIP 
It’s a Defense Against Trojan Attacks on Deep Neural Network by using Digital image 
processing, DNN by usage of Perturbation on training images to find the difference between 
the original image and the triggered image. It can mainly be used for dealing with images. 
The STRIP defense method is not that effective when compared with other defense 
methods like Neural cleanse methods when it comes to text and voice. Fig-5 Illustrates the 
process mechanism of STRIP. 
 Neural Cleanse:
The model is designed to detect the backdoor triggers and reconstruct the possible triggers 
by using mitigation techniques. Firstly, to detect if any backdoor attack exist .If yes, 
identifying the target label. Finally, after detecting rejecting the sample that has adversarial 
inputs and patching the model completely from backdoor attack. By assuming delta is 
minimum for the infected model, calculating the delta min for every single label in the 
model using the reverse engineering for entire unit. Then finding the label which has smaller 
delta value from all the labels by using outlier detection algorithms. 
This defense method was able to successfully detect the whether the model is infected 
.Then the trigger used, identifying the workflow of backdoor attack using reverse 
engineering trigger. After that finally removing the adversial inputs using the proactive filter 
and patching the backdoor attack via unlearing (training the DNN to make correct 
predictions when an input has reversed trigger.Fig-6 Illustrates the process mechanism of 
Neural Cleanse. 
Proposed Work: 
 The first objective of this research project is to built CNN model ie (clean model) and to 
make the model misclassified on selected targets .The model produced the accuracy rate of 
about 98%. 
 The second objective of the project is to inject backdoor trigger into the model in other 
words creating a poisonous triggered model using Deep learning ,CV tool to create own 
trigger. when the triggered inputs are passed and model should behave normally when 
the clean data is passed. 
 Firstly , creating full blank image of 28x28 using cv2 tool with trigger sixe 2x2. Randomly, 
select the pixel location from batch size(128) 10-20 random images. \item Selecting index of 
trigger i.e. to assigning pixel location between 26-27 where the trigger should be 
inserted.\item Set the trigger to white scale/patch i.e. color to 1.\item Selected ’7’ as the 
target label,Updating Batch size. \item Updating validation data from the same pixel location 
which is chosen above for injecting 10-20 randomly triggered images. \item Finally 
generated test reports for both clean and trojaned samples to maintain overall accuracy of 
the model in two scenarios.  
Conclusion: 
Majority of these attacks are found through the third party in the field of MLAAS. The research 
concepts discussed in this field are the work done 3 years back.In this report, we have summarized 
on the concepts of neural Trojan attacks, discussed on existing related work for Backdoors and its 
defense methods finding out the best suggest able method by surveying on different papers and 
implemented concept of Badnets considering the MNIST dataset in real time by building the clean 
model using CNN model with an model performance of about 98%, Creating Poisonous model with 
performance rate of 100% . Implementing defence technique STRIP to check for accuracy of the 
model and recover to orginal model with performance rate of 92%. 
Future Scope: 
This research project can be expanded by implementing the poison model in such a way which can 
defeat STRIP (defense method).
