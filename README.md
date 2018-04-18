# spark_streaming_study
used for big data programming course
## 1. Login the Azure

### 1.1 Directly login the Azure 
If you are in the school, you can directly access to Azure service using ssh:

```
  ssh MyFordhamIDname@10.223.36.8
```

The username and password is the same as the MyFordham.

### 1.2 Use Erdos to log in the Azure
If you are not in school, you might be not able to access to Azure directly, but you can link to the Erdos first.

```
  ssh ErdosName@erdos.dsm.fordham.edu
```
Once you login you now can login to the Azure

```
  ssh MyFordhamIDname@10.223.36.8
```



## 2. Get the files in github
And then please download the SentimenAnalysis files from github
```
  git clone https://github.com/weiyanwuda/spark_streaming_study.git
```

## 3. start your sentiment project

### 3.1 The structure of the program
First, we go into the project:
```
  cd spark_streaming_study
```
Now you get the whole project for sentimenanalysis, let us see the structure of the project:
```
  \
    build.sbt \\Don't change it, it concludes all the libaries and packages for this project
    
    src\main\scala\
                    SentimentAnalysis.scala  \\ The main part of program, you can try to use it to do what you want
                    
                    SentimentAnalysisUtils.scala  \\ The NLP libaries the main program used.
                    
                    StreamingExamples.scala  \\ This one just a test demo for the program, you can do what you want.
                    
    outputs\
                tags    \\ all the output of tags would save here
                
```

### 3.2 Run your program
How can we try to test our program? now go back to the root directory of the project, where you can find the build.sbt file in there, and type:

```
  "run YourTwitterConsumerKey YourTwitterConsumerSecret YourTwitterAccessToken YourTwitterAccessTokenSecret  Apple"
```

You can change the "Apple" to any word you want.<br/>
And you can get your twitter token in: https://apps.twitter.com/
