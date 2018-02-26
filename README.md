# road_lane_line_detection


## 1. Describe my pipeline. 

- My pipeline consisted of 5steps. I'm going to write details below.
1. I converted the images to grayscale.
2. Applying the images to gaussian_blur function to blur the images.
3. I applyed the images to canny function to detect the edge.
4. I masked partial of the images to delete place which is not lane.
5. And then I applyed the images to hough_line() function to detect straight line.
6. I used weighted_img() function to merge original iamge with line I detected.
7. Finnaly, I tested my solution on two provided videos.


## 2. Identify potential shortcomings with your current pipeline
- One potential shortcoming would be what would happen when the line interval is large, I could not detect the line.

## 3. Suggest possible improvements to your pipeline
- A possible improvement would be to decrease length of y2 (y2 = int((maxY/2)) + 60)
- if the left line interval is so large, draw_lines() function understand right line is next line.

## 4. Output videos
![Output_image](https://qiita-image-store.s3.amazonaws.com/0/45617/015bd058-7ea0-e6a5-b9cb-36a4fb38e59c.png "Qiita")


1. [solidWhiteRight](https://www.youtube.com/watch?v=7N8M5-Zdnzk&feature=youtu.be)
2. [solidYellowLeft](https://www.youtube.com/watch?v=ba81I_ywZ4Q&feature=youtu.be)
