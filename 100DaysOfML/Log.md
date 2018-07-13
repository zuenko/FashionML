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