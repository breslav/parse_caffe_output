Objective: Parse caffe's output during training into useable form, by extracting training/testing loss vs iterations.

parse_log.sh - The purpose of this shell script is to take the output generated by caffe during or after training and to automatically extract training iterations vs loss, and testing iterations vs loss. 

plot_train_test_loss.m - The purpose of this matlab script is to make a plot containing training loss vs iterations, and testing loss vs iterations.

Usage: 
1. First copy and paste the output of caffe into a text file called solver_log.txt.
2. Then in the same directory you should be able to run parse_log.sh by typing ./parse_log.sh (make sure permissions are set correctly)
3. The script should generate a folder called parsed_log which will contain the original log and four text files. The text files are split up into the training iterations, training loss, testing iterations, and testing loss.
4. The matlab script reads from the parsed_log folder whose path you need to specify by setting the file_path variable, and it generates a figure with training loss vs iterations in blue, and testing loss vs iterations in green. 
 

