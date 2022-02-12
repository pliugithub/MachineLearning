[Return to home page](./README.md) 

# Table of Contents

The course is taught in a sequence of units.  Each unit takes between one
and two weeks so that the entire class can be fit into a single semester.
Most units currently have four or five components:
* **Lecture Notes**:  These are slides accompanying the class lecture.  They include code snippets
   from the demos.   
* **Lecture Videos**:  The lecture videos are available on Brightspace.
* **Whiteboard**: [MS OneNote](https://1drv.ms/u/s!AhGPBmraRihnjy7q930t8ZWGk9Ch)
* **Demo**: These are python-based [Jupyter notebooks](http://jupyter.org/)
   for demonstrations given during the lectures.  Some demos have a
   component that is done in class.  The demos do not generally cover
   all topics, since some concepts are left for the students to figure out 
   for themselves in the labs.
* **Lab**:  Following the lecture, the students do a python-based exercise at home
   that builds on the demo.
   The labs in the repository are given as skeletons with `TODO`
   markers that the students fill in.
* **Problems**:  These are more analytic problems, also done at home.

The problem and lab solutions are provided to students enrolled in the class.
If you are an instructor
and wish copies of the solutions for yourself,
please contact Sundeep Rangan at <srangan@nyu.edu>.

* Syllabus: [Spring 2022](./lectures/GY6143_ML_Syllabus_S22.pdf)
   * [NYU Tandon Policies and Procedures on Academic Misconduct](https://engineering.nyu.edu/student-life/student-activities/office-student-affairs/policies/code-conduct#chapter-id-34265)

* Setting up python and jupyter notebook
    * [Using Google Colaboratory(Prefered Method)](./Basics/Colab.md)
    * [Set up a local machine(Need this to generate PDF for homework submissions)](./Basics/setup.md)
    * [Or set up a CPU or GPU virtual machine in Google Cloud Platform (Not recommended for beginners)](./GCP/getting_started.md)

 * Setting up github
    * [Downloading the course material from github](./Basics/github.md)

* Introduction
    * Course Admin [[pdf]](./lectures/CourseAdmin.pdf) [[Powerpoint]](./lectures/CourseAdmin.pptx)

    
* Unit 1:  What is machine learning? 
    * Lecture:  Introduction to Machine Learning [[pdf]](./lectures/Lect01_IntroML.pdf)
     [[Powerpoint]](./lectures/Lect01_IntroML.pptx)
     * Demo: [Github](./Basics/github.md)
     * Demo: [Setting up the environment on a local machine](./Basics/setup.md)
     * Demo: [Google Cloud Platform](./GCP/readme.md)
     * Demo: [Python Tutorial](./unit01_intro/Python_tutorial.ipynb)
     * Demo: [Introduction to numpy vectors](./unit01_intro/demo_intro_vectors.ipynb)
     * Demo: [Overview of Google Colab](./unit01_intro/Overview_of_Colaboratory_Features.ipynb)
     
* Unit 2:  Simple linear regression
    * Lecture:  Simple linear regression [[pdf]](./lectures/Lect02_SimpRegression.pdf)
     [[Powerpoint]](./lectures/Lect02_SimpRegression.pptx)        
    * Demo: [Understanding automobile mpg](./unit02_simp_lin_reg/demo_auto_mpg.ipynb)
    * Whiteboard: [MS OneNote](https://1drv.ms/u/s!AhGPBmraRihnjy7q930t8ZWGk9Ch)   
    * Homework (Due on Feb 8, 23:59 PM ET)
        * Problem: [[pdf]](./unit02_simp_lin_reg/prob/prob_simp_lin_reg.pdf)
        * Lab: [Boston housing data](./unit02_simp_lin_reg/lab_housing_partial.ipynb) (submit both .ipynb and .pdf files) 

* Unit 3:  Multiple linear regression
    * Lecture:  Multiple linear regression [[pdf]](./lectures/Lect03_MultLinRegression.pdf)
     [[Powerpoint]](./lectures/Lect03_MultLinRegression.pptx)
    * Demo 1: [Predicting glucose levels](./unit03_mult_lin_reg/demo1_glucose.ipynb)
    * Demo 2: [Python broadcasting(Optional)](./unit03_mult_lin_reg/demo2_python_broadcasting.ipynb)
    * Whiteboard: [MS OneNote](https://1drv.ms/u/s!AhGPBmraRihnjy7q930t8ZWGk9Ch)   
    * In-class Exercise: [Linear regression](./unit03_mult_lin_reg/linreg_inclass.ipynb)
    * Homework (Due on on Feb 15, 23:59 PM ET)
        * Lab: [Calibrating robot dynamics](./unit03_mult_lin_reg/lab_robot_calib_partial.ipynb)
        * Problems [[pdf]](./unit03_mult_lin_reg/prob/prob_mult_reg.pdf)

`------Materials below are outdated and will be updated before each class.------`

* Unit 4:  Model selection
    * Lecture:  Model selection [[pdf]](./lectures/Lect04_ModelSelection.pdf)
     [[Powerpoint]](./lectures/Lect04_ModelSelection.pptx)    
    * Demo 1: [Polynomial order selection with cross-validation](./unit04_model_sel/demo_polyfit.ipynb)
    * Demo 2: [Feature transforms and model validation(Optional)](./unit04_model_sel/demo2_transform.ipynb)
    * Homework (Due on Oct 6, 23:59 PM ET)
        * Lab: [Neural decoding motor cortex signals](./unit04_model_sel/lab_neural_partial.ipynb)          
        * Problems [[pdf]](./unit04_model_sel/prob/prob_model_sel.pdf)

* Unit 5:  Regularization and LASSO
    * Lecture:  LASSO Regularization [[pdf]](./lectures/Lect05_Lasso.pdf)
     [[Powerpoint]](./lectures/Lect05_Lasso.pptx)   
    * Demo 1: [Predicting prostate cancer](./unit05_lasso/demo1_prostate.ipynb)      
    * Demo 2: [Predicting housing prices](./unit05_lasso/demo2_housing.ipynb)
    * Homework (Due on Oct 13, 23:59 PM ET) 
        * Lab: [EEG source localization](./unit05_lasso/lab_eeg_partial.ipynb) 
        * Problems [[pdf]](./unit05_lasso/prob/prob_lasso.pdf) [[Latex]](./unit05_lasso/prob/prob_lasso.tex)

* [Unit 6:  Logistic regression](./unit06_logistic/readme.md)
    * Lecture:  Linear classification and logistic regression
    [[pdf]](./lectures/Lect06_LogisticReg.pdf)
    [[Powerpoint]](./lectures/Lect06_LogisticReg.pptx)        
    * Demo: [Breast cancer diagnosis via logistic regression](./unit06_logistic/demo_breast_cancer.ipynb)
    * Homework (Due on Oct 20, 23:59 PM ET) 
        * Lab: [Genetic analysis of Down's syndrome in mice](./unit06_logistic/lab_gene_partial.ipynb)
        * Problems: [[pdf]](./unit06_logistic/prob/prob_logistic.pdf)

* [Unit 7:  Nonlinear optimization](./unit07_optim/readme.md)
    * Lecture:  Nonlinear optimization and gradient descent
    [[pdf]](./lectures/Lect07_Optim.pdf)
    [[Powerpoint]](./lectures/Lect07_Optim.pptx)     
    * Demo 1: [Computing gradients](./unit07_optim/demo1_computing_gradients.ipynb)
    * Demo 2: [Simple gradient descent optimization](./unit07_optim/demo2_grad_descent.ipynb)    
    * Homework (No submission required! Solution will be released early for you to prepare for the exam.) 
        * Lab: [Nonlinear least squares material modeling](./unit07_optim/lab_nlls_partial.ipynb)
        * Problems: [[pdf]](./unit07_optim/prob/prob_optim.pdf)

* [Unit 8:  Support vector machines](./unit08_svm/readme.md)
    * Lecture:  SVM [[pdf]](./lectures/Lect08_SVM.pdf)
    [[Powerpoint]](./lectures/Lect08_SVM.pptx)       
    * Demo 1: [MNIST digit classification](./unit08_svm/demo_mnist_svm.ipynb)
    * Demo 2: [Visualizing kernels](./unit08_svm/demo2_kernels.ipynb)
    * Homework (Due on Nov 10, 23:59 PM ET) 
        * Lab: [Extended MNIST with letters](./unit08_svm/lab_emnist_partial.ipynb)    
        * Problems: [[pdf]](./unit08_svm/prob/prob_svm.pdf)

* [Unit 9: Neural networks with Keras and Tensorflow](./unit09_neural/readme.md)
    * Lecture:  Neural networks [[pdf]](./lectures/Lect09_NeuralNet.pdf)
    [[Powerpoint]](./lectures/Lect09_NeuralNet.pptx) 
    * Supplementary notes with solved problems [[pdf]](./unit09_neural/prob/supplementary_neural.pdf) [[Latex]](./unit09_neural/prob/supplementary_neural.tex)
    * Demo 1: [First neural network in Keras](./unit09_neural/demo1_synthetic.ipynb)
    * Demo 2: [MNIST neural network classification](./unit09_neural/demo2_mnist_neural.ipynb)
    * In-class:[Exercise](./unit09_neural/neural_inclass.ipynb)
    * Homework (Due on Nov 17, 23:59 PM ET) 
        * Lab: [Music instrument classification](./unit09_neural/lab_music_partial.ipynb)
        * Problems: [[pdf]](./unit09_neural/prob/prob_neural.pdf)


* [Unit 10:  Convolutional and deep networks](./unit10_cnn/readme.md)
    * Lecture:  Convolutional and deep networks
    [[pdf]](./lectures/Lect10_ConvNet.pdf)
    [[Powerpoint]](./lectures/Lect10_ConvNet.pptx)         
    * [Setting up a GPU instance](./GCP/getting_started.md) (Recommended)
    * [Demo 1: 2D convolutions and convolutional layers in keras](./unit10_cnn/demo1_convolutions.ipynb)
    * [Demo 2: Creating an image set using the Flickr API](./unit10_cnn/demo2_flickr_images.ipynb)
    * [Demo 3: Exploring the deep VGG16 network](./unit10_cnn/demo3_vgg16.ipynb)
    * [Demo 4: Building an image classifier using CIFAR10 dataset](./unit10_cnn/demo4_classifier.ipynb)
    * [Demo 5: Building an autoencoder for image denoising using CIFAR10 dataset](./unit10_cnn/demo5_autoencoder.ipynb)
    * Homework (Due on November 24, 23:59 PM ET) 
        * Lab: [Transfer learning with a pre-trained network](./unit10_cnn/lab_fine_tune_partial.ipynb)
    (GPU recommended)
        * Problems: [[pdf]](./unit10_cnn/prob/prob_cnn.pdf)


* [Unit 11:  PCA](./pca/readme.md)
    * Lecture:  PCA [[pdf]](./lectures/Lect11_PCA.pdf) [[Powerpoint]](./lectures/Lect11_PCA.pptx)          
    * [Demo 1:  PCA eigen-faces-SVM](./unit11_pca/demo1_eigen_face.ipynb)
    * [Demo 2:  Low-rank matrix completion via embedding layers](./unit11_pca/demo2_low_rank.ipynb)
    * Homework (Due on December 1, 23:59 PM ET) 
        * Lab: [PCA with hyper-parameter optimization](./unit11_pca/lab_wine_partial.ipynb)
        * Problems: [[pdf]](./unit11_pca/prob/prob_PCA.pdf)


* [Unit 12:  Clustering and EM](./unit12_cluster/readme.md)
    * Lecture:  Clustering and EM [[pdf]](./lectures/Lect12_Clustering.pdf)
    [[Powerpoint]](./lectures/Lect12_Clustering.pptx)         
    * [Demo 1: Document clustering via k-means and latent semantic analysis](./unit12_cluster/demo1_doc_cluster.ipynb)
    * [Demo 2: Color quantization via k-means and EM-GMM](./unit12_cluster/demo2_kmeans_GMM_color_quantization.ipynb)  
    * Homework (Due on December 8, 23:59 PM ET)   
        * Problems: [[pdf]](./unit12_cluster/prob/prob_clustering.pdf)

* Unit 13:  Decision Trees and Random Forest
    * Lecture:  Decision tree and random foreast [[pdf]](./lectures/Lect13_Trees.pdf)
    [[Powerpoint]](./lectures/Lect13_Trees.pptx)         
    * [Demo: Prediction of temperature using decision tree and random forest](./unit13_tree/decision_tree_and_random_forest.ipynb)
    * Homework (***Will NOT be graded***)   
        * Homework [[pdf]](./unit13_tree/prob/prob_tree.pdf)
        

* Final Exam
    * :bell::bell::bell: Final Exam will be on Dec 15 @6PM.

* [Course Project](./projects/readme.md)
    * Course project is OPTIONAL. It consists 20% of your total grade. If you choose not to do it, I will take the higher grade of your midterm and final exams, and use it for your project grade.
    * One or two students in a project group.
    * List of suggested project topics can be found [here](./projects/readme.md). 
        * Recently published paper + existing code as a starting point for your projects.
        * You are free to choose a topic not listed here.
    * What do we expect?
        * The project to be different than something you can directly find in a blog post or Kaggle. You should always add references to data/code/sentences you copied online.
        * You can try to improve the accuracy reported in a blog post; 
        * You can train on additional data and test on real-world data that you collected yourself;
        * You can change the model, try parameter optimization etc; 
        * You can compare different models and report their success, what kind of datapoints are usually missed with what models etc;
        * If you cannot make improvements, tell us why it failed and what are the lessons learned.
    * :bell::bell::bell: Project report is due on the Dec 22, 23:59 PM ET.
        * Submit your code and report on Gradescope;
        * Follow the submission guidelines listed [here](./projects/submission.md)
        * Make sure we can duplicate your results. If you used some data that is not publicly available online, please upload to Google drive/Dropbox/Github so that we can access it;
        * You need a quad chart at the begining of your report, which serves as an executive summary. You need to very briefly describe what is the motivation, why it should be solved by ML and the tool you picked,  what is your contribution (how is it different the existing), results, summary/future directions/lessons learned. Be concise!
        * The report should be formated as a paper of few pages long. 
    * Doing a project will never hurt your grade (assuming you didn't do any plagiarism on the project). If project grade is lower than your exams, we will use your exams for that 20% portion and not consider the project.
    * Make sure you don't plagiarise. Please clearly cite the sources you use for your work whether it is a blog post or github repository or a paper published. It is very important you don't miss any source you used. This class and NYU take plagiarism very seriously. If plagiarism is detected you will get a ZERO grade from the project. ( You can definitely use a blog post or a github repository as a starter code: Cite it, clearly write what is the difference of your work from the starter code and how did you contribute.)


        












    

    







