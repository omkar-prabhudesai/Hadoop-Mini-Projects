
# Yelp Data (Academic) processing with Hadoop and Hive

* Importing Data into HDFS
      1. Create the required directories into HDFS as follows -
      ```
          hdfs dfs -mkdir -p /user/cloudera/rawdata/yelpds/businesses
          hdfs dfs -mkdir -p /user/cloudera/rawdata/yelpds/reviews
          hdfs dfs -mkdir -p /user/cloudera/rawdata/yelpds/tips
          hdfs dfs -mkdir -p /user/cloudera/rawdata/yelpds/users
          hdfs dfs -mkdir -p /user/cloudera/rawdata/yelpds/checkins
          ```
     2. Copy the corrusponding dataset files to respective directories -     
          ```
          hdfs dfs -moveFromLocal yelp_academic_dataset_review.json /user/cloudera/rawdata/yelp/reviews
          hdfs dfs -moveFromLocal yelp_academic_dataset_business.json /user/cloudera/rawdata/yelp/businesses
          hdfs dfs -moveFromLocal yelp_academic_dataset_tip.json /user/cloudera/rawdata/yelp/tips
          hdfs dfs -moveFromLocal yelp_academic_dataset_user.json /user/cloudera/rawdata/yelp/users
          hdfs dfs -moveFromLocal yelp_academic_dataset_checkin.json /user/cloudera/rawdata/yelp/checkins
         ```
  
