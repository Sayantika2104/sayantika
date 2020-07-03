# Artificial Intelligence
In this challenge, I was supposed to crop the given image by mask. 
Firstly, I imported the necessary libraries such as OpenCV(cv2), numpy and matplotlib.
Then I read the required image files and their respective masks with the help of cv2.imread().
I resized the original image files so as to match the dimensions of their respective masks.
Then I completed the given function crop_by_mask. I calculated the inverse of the mask so as to bring the black portion inside and the white part outside. The image will be displayed in the black part.
Then I performed bitwise or operation on the inversed mask and the resized image. This made the image to be displayed on top of the inversed mask image. But the background remains white.
To convert the white background to black, I anded the foreground with the original mask image using bitwise_and operation.
Then return the background.
Now I passed the resized image and the mask as parameters of crop_by_mask function. The plt.imshow() displays the required image.
