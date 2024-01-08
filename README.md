
## Diagnosis of disease from Optical Coherence Tomography (Classification)

<img src="https://github.com/rumeysakocc/OCT-Diagnostic-Model-and-Interface/assets/115664157/74ce8d97-2051-477a-ad3a-51b903f895f7" alt="images" align="left" width="400" height="300">

<p>OCT stands for optical coherence tomography. This is a technique that uses light waves to image the photosensitive tissue at the back of the eye.
Different layers and thicknesses of the eye can be measured with OCT. 
OCT is used in the diagnosis and follow-up of eye diseases such as retina and cornea[2]

In the 21st century, the development of optical coherence tomography (OCT) has revolutionised the ability to diagnose macular diseases and assess the necessity and effectiveness of treatments. It has become one of the most commonly performed medical imaging procedures, with approximately 30 million OCT scans performed each year worldwide. OCT imaging has now become the standard to guide the diagnosis and treatment of age-related macular degeneration (AMD) and diabetic macular oedema, the leading causes of preventable blindness worldwide.[2]</p>

## Classes

✓ **DME** stands for diabetic macular oedema. This is a complication of a condition called diabetic retinopathy. 
Diabetic retinopathy is damage to the small blood vessels of the retinal layer at the back of the eye. DME is the accumulation of fluid leaking from these damaged vessels in the macula area in the centre of the retina. The macula helps us to see objects in front of us clearly.[1]


✓ **CNV** stands for choroidal neovascularisation. This is an abnormal growth of blood vessels from the choroidal layer at the back of the eye into the retinal layer. CNV can be a result of certain eye diseases, such as age-related macular degeneration (AMD).


✓ **DRUSEN** are small, yellowish deposits that accumulate under the retina at the back of the eye. Drusen can be a symptom of some eye diseases, such as age-related macular degeneration (AMD). Drusen can impair the visual function of the retina or cause damage

## Data Set
In this project, the dataset used in the study "Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning"[3] in ScienceDirect was used. The use of this dataset is due to the large number of images, as well as the fact that the classification of the images was performed by 3 different eye specialists, the error in data classification is low. 
There are 90k data in the dataset with 4 classes in total.The dataset is available here[4].

## Objective and Result
This project is a diagnostic interface that takes any number of images from the user and shows which class (NORMAL, DME, CNV and DRUSEN) the image belongs to with percentages.

In order to run this interface on your computer, model training using the data set is required first.(OCT/ModelTraining.ipynb)

The model training took 35 hours by applying 8 epochs on 90k data and a success rate close to 96% was achieved. 
I recommend you to do your model training with a single epoch. Because the success you will get from a single epoch is also sufficient for the model. You can see the results below.
![result](https://github.com/rumeysakocc/OCT-Diagnostic-Model-and-Interface/assets/115664157/b1edb6ac-3ebc-4f6b-8724-f13296076fd7)

<img src="https://github.com/rumeysakocc/OCT-Diagnostic-Model-and-Interface/assets/115664157/aaeff7a3-3e85-4dc3-aa48-f47dd90d6f98" alt="images" align="left" width="400" height="250">

At the end of the model training, the most successful of the weight files is selected and the interface is given.

(OCT/Diagnostic_Interface.ipynb) Since we do not have a configuration file for the weight file to work on the interface, 
EfficientNet uses it by creating a model using the B5 architecture.
If you wish, you can give this model to the code as a config file.


Thus, you will have a simple OCT diagnostic interface. 


Waiting for your FeedBack


## References 

[1] https://eyewiki.aao.org/Diabetic_Macular_Edema

[2]https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04001-1

[3] https://www.sciencedirect.com/science/article/pii/S0092867418301545

[4] https://data.mendeley.com/datasets/rscbjbr9sj/2

