Download Link: https://assignmentchef.com/product/solved-computer-vision-i-project-3
<br>
<span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif; font-size: 2.61792em; letter-spacing: -1px;">Dense Optical Flow</span>

In this project you will implement the Lucas-Kanade method for estimating dense optic flow from a pair of images. The input is a pair of greyscale images taken from a video sequence, and the output will be two matrices containing the x and y components of the flow vector at each pixel.

To summarize the LK algorithm for computing flow:

<ol>

 <li>Read image1 and image2, and convert to double flow greyscale image frames.</li>

 <li>Compute the spatial intensity gradients <em>I<sub>x </sub></em>and <em>I<sub>y </sub></em>of image2. Recall that it is a good idea to smooth before taking the derivative, for example by using derivative of Gaussian operators.</li>

 <li>Compute the temporal gradient <em>I<sub>t </sub></em>by subtracting a smoothed version of image1 from a smoothed version of image2.</li>

 <li>For a given window size <em>W</em>, form a system of linear equations at each pixel by summing over products of gradients in its neighborhood, as specified by the Lucas-Kanade method. That is, at each pixel, you will have a set of equations:</li>

 <li>Solve for the flow vector [<em>u,v</em>] at each pixel. It is convenient to represent this vector field by two images, one containing the u component, and the other the v component of flow.</li>

 <li>Display the flow vectors overlaid on the image. You can use matlab “quiver” to show the flowfield.</li>

 <li>Another way to represent optical flow is to color code the flow vectors: direction of the vectoris coded by hue, and length of the vector is coded by saturation. Display your flow vectors using this method also.</li>

 <li><strong>Project Requirements:</strong></li>

</ol>

<ul>

 <li>Write a program to implement the above algorithm. Create a two level pyramid and foreach level of the pyramid compute the optical flow independently. Sample sequences to test your program will be available in blackboard.</li>

 <li><strong>Write a report. </strong>The report should include:

  <ol>

   <li>Abstract, description of algorithms, experiments, values of parameters used (Howdoes the size of W affect your results?), observations and conclusions.</li>

   <li>A FLOWCHART, input and optical flow images.iii. An appendix with your source code</li>

  </ol></li>

</ul>


