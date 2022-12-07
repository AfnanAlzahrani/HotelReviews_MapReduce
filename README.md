# HotelReviews_MapReduce

<img src="https://drive.google.com/uc?export=view&id=1ANzBFTLiElGdY4Bq9WwQN8I8kPViAZDL"/>


## Review

### Dataset:
> * The Hotel Reviews dataset contains two columns and 20491 row.


### Columns are:
> * Review: description of the experiment.
> * Rating: integers from 1 to 5, where 5 is the best and 1 is the worst.


### Problem statement:
> * A hotel intends to do maintenance based on the rating; If the most of customers rated less than three stars, the maintenance will be done by the end of the year; otherwise, it will be done later.
So, we used MapReduce to count the number of reviews for each rating(1,2,3,4,5) in the dataset.


### Implementation Steps:
#### Step 1: Transform raw data into key/value pairs in parallel.
The mapper will get the data file and make the Rating the key and the values will be the reviews. We will add number 1 for reviews.
#### Step 2: Shuffle and short by the MapReduce model.
The process of transferring mappers’ intermediate output to the reducer is known as shuffling. It will collect all the reviews(number 1s) together with the individual key and it will sort them. it will get sorted by key.
#### Step3: Process the data using Reduce.
Reduce will count each value(number 1) for each key.






## :octocat:	Team Memebers

- [Abdullah Huwaishel](https://github.com/hush966)
- [Afnan Alzahrani](https://github.com/AfnanAlzahrani)
- [Jumana Almussa](https://github.com/jumana0)
- [Mahmuod Alhassan](https://github.com/alhassanm)
- [Amjad Almusallam](https://github.com/ASM650)



# SDA - Hadoop - CodingDojo - MapReduce
