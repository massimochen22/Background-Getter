# Background-Getter

The program goes through all the input .ppm files and will get each pixels color data. 
The output will be cleared.ppm 

## Logic
The main part has to iterate through each pixels in the image, so it will be (width x height), the colors (r x g x b data), and through the number of images.
Everytime the program gets the color data of one pixel of one frame, it sums it to the value of the same color pixels in the other frames (so you will have the total value of the color data in tot number of frames), and then divide by the number of frames to obtain the average of it.

Once we know the average of a pixel we can tell which pixel value are not "close" to the average value hence understand also the "noisey" pixels.
The sample imput are in the "frames" folder, and they are a total of 17 files. In the input example below I just put 3 frames for demonstration purposes. The program ran with all the 17 files; the output below is the result of all 17 files input.

If using other .ppm files, the program would work only if the frames have the same size, and if a part of the background is present in most of the frames.

Input 1:
![Screen Shot 2022-02-13 at 11 21 18 PM](https://user-images.githubusercontent.com/89932323/153799524-66f1bce5-7fa2-451a-8767-d71ea6d3d9e0.png)
Input 2:
![Screen Shot 2022-02-13 at 11 19 23 PM](https://user-images.githubusercontent.com/89932323/153799437-18708279-5678-42b9-83bc-aa52541a8334.png)
Input 3:
![Screen Shot 2022-02-13 at 11 19 10 PM](https://user-images.githubusercontent.com/89932323/153799439-b3555a25-11de-4eee-a9b9-a7652e550534.png)

Output:
![Screen Shot 2022-02-13 at 11 18 35 PM](https://user-images.githubusercontent.com/89932323/153799283-b62ccd60-8d8a-450b-851e-d4766145f80d.png)


