# Breast_cancer_detection_Using_Neural_nets
What is the Project all about?
In India and over the world, Cancer has become a deadly disease and more and more people are suffering from Cancer and a survey says one in every 30 women suffer from this disease in their lifetime and so basically the project was first thought of because of the increase in cases of breast cancer and one thing which is very important that if we can detect the Cancer at an early stage then there is an increased chances of it getting cured.So this project lays a foundation in making the detection of the cancer automated so that more and more people can get it diagonised early so as get cured.

How it is implemented?
The signs of detection are Masses and micro calcification clusters which are important in early detection of breast cancer.

Micro calcification are nothing but tiny mineral deposits within the breast tissue. They look similar to small white colored spots. They may or may not be caused by cancer.

Masses can be many things, including cysts (fluid-filled sacs) and non-cancerous solid tumors, but they could also be cancerous.

The difficulty in cancer detection is that the abnormalities from normal breast tissues are hard to read because of their subtle appearance and ambiguous margins.Automated tools which can help radiologist in early detection of breast cancer.

Further we have classified the cancer into three categories after its detection- Normal,Malignant,Benign.

Methodology
We​ ​have​ ​used​ ​adaptive​ ​mean​ ​filter​ ​to​ ​remove​ ​noise​ ​from​ ​image.​ ​since​ ​it​ ​is​ ​better among​ ​all​ ​the​ ​spatial​ ​filters​ ​and​ ​distinguish​ ​fine​ ​details​ ​from​ ​noise.​​The​ ​Adaptive Median​ ​Filter​ ​performs​ ​spatial​ ​processing​ ​to​ ​determine​ ​which​ ​pixels​ ​in​ ​an​ ​image have​ ​been​ ​affected​ ​by​ ​impulse​ ​noise.​ ​The​ ​Adaptive​ ​Median​ ​Filter​ ​classifies​ ​pixels as​ ​noise​ ​by​ ​comparing​ ​each​ ​pixel​ ​in​ ​the​ ​image​ ​to​ ​its​ ​surrounding​ ​neighbor​ ​pixels.

The​ ​size​ ​of​ ​the​ ​neighborhood​ ​is​ ​adjustable,​ ​as​ ​well​ ​as​ ​the​ ​threshold​ ​for​ ​the comparison.​ ​A​ ​pixel​ ​that​ ​is​ ​different​ ​from​ ​a​ ​majority​ ​of​ ​its​ ​neighbors,​ ​as​ ​well​ ​as being​ ​not​ ​structurally​ ​aligned​ ​with​ ​those​ ​pixels​ ​to​ ​which​ ​it​ ​is​ ​similar,​ ​is​ ​labeled​ ​as impulse​ ​noise.

​These​ ​noise​ ​pixels​ ​are​ ​then​ ​replaced​ ​by​ ​the​ ​median​ ​pixel​ ​value​ ​of the​ ​pixels​ ​in​ ​the​ ​neighborhood​ ​that​ ​have​ ​passed​ ​the​ ​noise​ ​labeling​ ​test.we​ ​are initially​ ​converting​ ​the​ ​image​ ​into​ ​grayscale​ ​image​ ​using​ ​rgb2gray()​ ​function​ ​then ​​applying​ ​adaptive​ ​mean​ ​filtering​ ​to​ ​the​ ​resulting​ ​image​ ​and​ ​then​ ​converted​ ​the image​ ​into​ ​unsigned​ ​integer​ ​8​ ​using​ ​unit8()​ ​function.

​In​ ​this​ ​way​ ​we​ ​preprocessed image.then​ ​we​ ​performed​ ​GMM​ ​segmentation(Gaussian​ ​Mixture​ ​Model)​ ​on​ ​the preprocessed​ ​image​ ​with​ ​number​ ​of​ ​regions​ ​2​ ​and​ ​number​ ​of​ ​GMM​ ​components 2​ ​and​ ​maximum​ ​number​ ​iterations​ ​10.​ ​we​ ​performed​ ​k-means​ ​segmentation​ ​with k=2.​ ​then​ ​we​ ​Implemented​ ​HMRF-EM​ ​(Hidden​ ​Markov​ ​Random​ ​Field​ ​Model)​ ​and its​ ​Expectation-Maximization​ ​Algorithm.

Difference between Malignant and Benign tissues in Breast
![cancer2](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/3f49efd1-e601-4a72-8098-3973f2efd7ba)


Block Diagram of the Project
![cancer](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/92a04a19-708c-44af-83b5-b84156fe749a)

Preview

How to make the project work?
Open the project in matlab and then run guidemo and then a gui mode window will open and then just follow the steps there.For further information check the screenshots.

References
Anuj Kumar Singh and Bhupendra Gupta “A novel approach for breast cancer detection and segmentation in mammography ” Expert System With Applications 42(2015)990-1002.

J. Dheeba, N.Albert Singh, S. Tamil Selvi “Computer-aided detection of breast cancer on mammograms: A swarm intelligence optimized wavelet neural network approach” Journal of Biomedical Informatics (2014).

Project Owner
Keshav Mangal

Screenshots
Now you have to browse the image of the mammograms and give it as an input 
![Screenshot (12)](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/c2af3b20-3fa4-4123-8090-6133ee1091ca)
![Screenshot (13)](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/ae2794ec-4f88-46f1-a0b8-e795abdcb8bf)
![Screenshot (14)](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/8494969d-378f-4bb6-b8f3-c6a0052ae1a0)
![Screenshot (15)](https://github.com/keshavmangal/Breast_cancer_detection_Using_Neural_nets/assets/117340691/27718d21-ddcc-4ac2-8530-cad735e5c017)



In this step adaptive mean filtering is done Preview

GMM Segmentation is done Preview

So you can see one as the output in the right side which depicts that the cancer is benign Preview
