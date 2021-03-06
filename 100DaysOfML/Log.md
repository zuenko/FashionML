# 100 Days Of ML - LOG

## Day 0 : July 7 , 2018
 
**Today's Progress** : I have setup all the things I needed to complete this challenge and also completed choosing the projects I will work on.

**Thoughts** : Hope this will be exciting, will help me in Machine Learning in a more effective way. First of all, I need to find good dataset or make it. 


**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)


## Day 1 : July 8 , 2018
 
**Today's Progress** : For a couple of hours trying to figure out how to use a scrapy tool. It's much more complicated than you might think at the first time. Now reading and testing http://scrapingauthority.com/scrapyfundamentals/ , and hope that will help.

**Thoughts** : Fear about that tool, licnce and so on. Hope the data I will parse not protected by law :). I almost got the point about parsing the image, need to sync it with additional categorical data. And do I really need that? Tomorrow will read about DeepFashion thoroughly. And hope I'll download it finally.
    
    Plans:
        - Get photo of users clothes.
        - Categorize it.
        - Great looks with categories.
        - Then use ensembles to predict look, or find familiar look.

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)


## Day 2 : July 9 , 2018
 
**Today's Progress** : Picked [DeepFashion (Category and Attribute Prediction Benchmark)](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion/AttributePrediction.html) dataset as the best one in my field. I've readed about cnn, object Detection, speed and accuracy comparing and so on. Installed darknet, watched videos about training and all that stuff. 

**Thoughts** : Want to figure out how to make dataset with good clothes combination, stylists? Also, yolo seemed pretty accurate and fast, but ssd pretty tough and mobilenet the fastest. And if I make the combination, can we actually use classic trees models or we need deep learning in that? So I have changed:
    
    Plans:
    	- Figure out how to make combination dataset.
    	- What about gans?
    	- Plan demo?
        - Is it possible to use ensembles to predict look, or find familiar look?

    Demo plan:
    	- Make demo
    	- ???
    	- Profit!

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)


## Day 3 : July 10 , 2018
 
**Today's Progress** : My plans now in trello, so I can easilly set deadlines and watch my progress. I understand how to train yolo, still preparing attributes .csv and bbox. Bbox location in DeepFashion, like "x_1" and "y_1" represent the upper left point coordinate of bounding box, "x_2" and "y_2" represent the lower right point coordinate of bounding box. Bounding box locations are listed in the order of [x_1, y_1, x_2, y_2]. So I need to convert them into <x> <y> <width> <height> - float values relative to width and height of image, it can be equal from (0.0 to 1.0]

**Thoughts** : First time with yolo, that should be interesting. I looked at Fashion Synthesis Benchmark and read paper, funny results:-), but pretty far away from my target. Don't want to use colab for training, so need to find a server for a couple days(or hours). Every day I try to put more time in 100DaysOfML, because compare to main work, less time, less results are anoying me.  

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)

## Day 4 : July 11 , 2018
 
**Today's Progress** : Still extracting features from annotation, pretty tough when your computer doesn't have enough memory. Working on solution. Founded annotation to yolo coordinates:

![GitHub Logo](https://i.redd.it/6unjoj3jkmx01.png)

- [x] list_eval_partition
- [x] list_category_img
- [x] list_bbox
- [ ] list_attr_img

**Thoughts** : I'll have more time at holidays, hope that I'll done label data, before them. 

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)


## Day 5 : July 12 , 2018
 
**Today's Progress** : Merged almost all annotation(except atr), made yolo labels.

**Thoughts** :  Still not enough memory for atr_labels, thinking about sparse matrix. Need to plot yolo box and compare to original. Yolo labels calculated with images height and width, hence shape of images may be different in img_highres and img datasets.

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)


## Day 6 : July 13 , 2018
 
**Today's Progress** : Atributes annotation done, dtypes yay! I plotted box with yolo labels, so yep, it not working, or plotter is bad. 

**Thoughts** :  Find out how to plot, what resolution of images. 

**Link to work:** [Fashion ML](https://github.com/zuenko/FashionML)

## Day 7 : July 14 , 2018
 
**Today's Progress** : Still try to find best solution for converting. With img_highres all fine, plotted original coordinates. Also made another repository where I'll implement ML algo, while training and other stuff.  

**Thoughts** :  Perhaps something wrong in plotter. I've tried different computation for yolo, but everything seemd logical.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)
- [Ml_algo_from_scratch](https://github.com/zuenko/Ml_algo_from_scratch)

## Day 8 : July 15 , 2018
 
**Today's Progress** : Done testing! All works fine, finaly! Working out on yolo format for training and testing. And I'm writing an article about my progress.
Done:
- [x] Yolo labels
- [x] Ploting
- [x] Converting
- [x] testing

**Thoughts** : Need to understand how to store labels for image, as I saw in the instruction that we need .txt file for each image, but where should we put that? What is .data and .names? 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 9 : July 16 , 2018
 
**Today's Progress** : Prepared yolo files, started to train, but got a couple of problems. That thing try to cath files that doesn't exist :-)

**Thoughts** : That pathes not inside, need to check train.txt, test.txt. And preparation script.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 10 : July 17 , 2018
 
**Today's Progress** : Solving problems with zero loss, nans etc. In process of training.

**Thoughts** : Mybe I need to switch from darknet tool to another? Because I'm not the only one who has a problems with that tool. Creat an issue in github and google group. 
Links:
- [Github](https://github.com/pjreddie/darknet/issues/980)
- [Google Group](https://groups.google.com/forum/#!topic/darknet/yBPBEXRDhKY)

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 11 : July 18 , 2018
 
**Today's Progress** : Solving problems with zero loss, nans etc. In process of training. Same as before. Writing article.

**Thoughts** : Mybe I need to switch from darknet tool to another? Because I'm not the only one who has a problems with that tool. Creat an issue in github and google group. 
Links:
- [Github](https://github.com/pjreddie/darknet/issues/980)
- [Google Group](https://groups.google.com/forum/#!topic/darknet/yBPBEXRDhKY)

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 12 : July 19 , 2018
 
**Today's Progress** : Tired of yolo. Today, I watched a couple courses about deep-learning, read papers about another architecture, youtube reviews of them and so on. Today is the research day.

**Thoughts** : SSD might be useful or fast rcnn, need to check tensorflow's models.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 13 : July 20 , 2018
 
**Today's Progress** : Learning about yolo, caffe, pytorch. For now, I'm comparing each model, because we don't need low fps. 

**Thoughts** : Hope ssd will solve my problem.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 14 : July 21 , 2018
 
**Today's Progress** : Find a couple implementations of SSD (single shot detector), installed all depencies.

**Thoughts** : Loking for good tf implementation, but fps in a different ranges.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 15 : July 22 , 2018
 
**Today's Progress** : Reinstalled ubuntu. With good cuda drivers. Watched lectures about pytorch.

**Thoughts** : Hate that feeling, when there are no good implementation. 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 16 : July 23 , 2018
 
**Today's Progress** : Learning pytorch, reading Goodfellow.

**Thoughts** : Testing ssd, a bit.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 17 : July 24 , 2018
 
**Today's Progress** : Learning pytorch, reading Goodfellow.

**Thoughts** : Testing ssd, a bit.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 18 : July 25 , 2018
 
**Today's Progress** : Fixed yolo, trying to find GPU server for free.

**Thoughts** : CPU may be too slow for me.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 19 : July 26 , 2018
 
**Today's Progress** : Something wrong with yolo, checking again.

**Thoughts** : Whats wrong, again.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 20 : July 27 , 2018
 
**Today's Progress** : Training yolo, tuning hyperparams.

**Thoughts** : Thinking about other models.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)


## Day 21 : July 28 , 2018
 
**Today's Progress** : Training yolo, tuning hyperparams.

**Thoughts** : Thinking about other models.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)


## Day 22 : July 29 , 2018
 
**Today's Progress** : Training yolo, tuning hyperparams. Learning basics, couresra into to deep-learning.

**Thoughts** : Thinking about other models.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)


## Day 23 : July 30 , 2018
 
**Today's Progress** : I stopped training and testing yolo. A lot of problems, accuracy not improving. Played with lr and other params, same thing. 

**Thoughts** : Tensorflow models figuring out how to implement object detection.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 24 : July 31 , 2018
 
**Today's Progress** : Learning [Intro-to-deep-learning](https://www.coursera.org/learn/intro-to-deep-learning)

**Thoughts** : fast.ai? 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 25 : August 1, 2018
 
**Today's Progress** : Continue learning [Intro-to-deep-learning](https://www.coursera.org/learn/intro-to-deep-learning)

**Thoughts** : Tasks a bit complicated

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 26 : August 2, 2018
 
**Today's Progress** : Continue learning [Intro-to-deep-learning](https://www.coursera.org/learn/intro-to-deep-learning)

**Thoughts** : Towards data science on medium help me with understanding.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 27 : August 3, 2018
 
**Today's Progress** : Pytorch day and lectures

**Thoughts** : Need to do something with learning yolo. Maybe pic not good enough.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 28 : August 4, 2018
 
**Today's Progress** : Goodfellow deep-learning intro-to-deep-learning

**Thoughts** : Reading about tasks in computer vision - good idea.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 29 : August 5, 2018
 
**Today's Progress** : Pytorch day

**Thoughts** : Research day.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 30 : August 7, 2018
 
**Today's Progress** : Pytorch day and lectures

**Thoughts** : Deep-Learning book notes are perfect for understanding math deeply.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 31 : August 8, 2018
 
**Today's Progress** : Goodfellow day

**Thoughts** : Reading notes.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 32 : August 9, 2018
 
**Today's Progress** : Goodfellow day

**Thoughts** : Reading notes.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 33 : August 10, 2018
 
**Today's Progress** : Goodfellow day

**Thoughts** : Reading notes.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 33 : August 11, 2018
 
**Today's Progress** : Intro-to-dl day. Learned about auto-encoders.

**Thoughts** : Reading notes.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 34 : August 12, 2018
 
**Today's Progress** : Intro-to-dl finished 4 week, learned about GANs.

**Thoughts** : Reading notes.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 35 : August 13, 2018
 
**Today's Progress** : Reading articles and watching videos about pytorch. Experimenting with yolo 

**Thoughts** : New config in yolo, called - yolov3-spp, let's try it.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 36 : August 14, 2018
 
**Today's Progress** : Training yolo. 

**Thoughts** : Preparing for article writing. 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 37 : August 15, 2018
 
**Today's Progress** : Training yolo. 

**Thoughts** : Preparing for article writing. 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 38 : August 16, 2018
 
**Today's Progress** : Yolo not improving, looking forward just classification methods. 

**Thoughts** : Maybe something wrong with my labels.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 39 : August 17, 2018
 
**Today's Progress** : Start first experiments with pytorch

**Thoughts** : Lectures are very helpfull.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 40 : August 18, 2018
 
**Today's Progress** : Tensorboard+pytorch

**Thoughts** : A lot of various tools around for visualization.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 41 : August 19, 2018
 
**Today's Progress** : Overview inside the dataset.  

**Thoughts** : Something wrong with dataset, I don't know the purpose of boxes. 

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 42 : August 20, 2018
 
**Today's Progress** : First nn in pytorch. 

**Thoughts** : Just amazing tool.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)

## Day 21 : August 21, 2018
 
**Today's Progress** : Start writing transfer learning for deepfashion.

**Thoughts** : Want to do good dataset prepartion.

**Link to work:** 
- [Fashion ML](https://github.com/zuenko/FashionML)
