Download Link: https://assignmentchef.com/product/solved-cs148-homework-4-ray-tracing
<br>
Introduction to Computer Graphics and Imaging (Summer 2012), Stanford University Due Monday, July 30, 11:59pm

As promised, since this homework was not announced on the original CS 148 syllabus, it is a bit shorter and more open-ended than the other homeworks for this course. Even so, be sure to get an early start to make sure everything compiles and to reserve enough time to add all the features we’re requesting.

In this homework, you will be adding some features to a barebones ray tracer using techniques we have discussed in lecture. Unlike our other assignments, we will be leaving nearly all of the software engineering, implementation, and structuring decisions to you.

The ray tracer provided in hw4.zip provides only the simplest functionality. Be sure to read through the following files before beginning the assignment:

<ul>

 <li>h/cpp: Provides simple functionality for writing .png images; requires libpng to compile.</li>

 <li>h/cpp: Stores the objects in a scene and performs basic ray tracing.</li>

 <li>h/cpp: An abstract class for representing a shape; also defines Ray and HitRecord structs.</li>

 <li>h/cpp: An example child class of Shape.</li>

 <li>cpp: The entry point for the program. Sets up a scene, initiates ray tracing, and saves the output.</li>

</ul>

For convenience, we have included the Eigen library for linear algebra. You can see samples of the library in use for processing three-dimensional vectors within the code; visit <a href="http://eigen.tuxfamily.org/">eigen.tuxfamily.org </a>for full documentation. Eigen is used in many important libraries, so it’s worth exploring a bit!

As you work on this project, you will be adding several classes that do not currently exist. You should add appropriate files in the src/ and include/ directories and modify the Makefile accordingly. As usual, this assignment has been tested on the Myth machines, although the code is simple enough that it should work in most environments with little modification; please check that it works on Myth before submitting.

For the assignment, please make the following changes to the ray tracer:

<strong>Problem 1 </strong>(15 points)<strong>. </strong><em>The ray tracer currently only can draw spheres. Add at least two more shapes. Potential options include other primitives, smooth surfaces with closed form equations f</em>(<em>~</em><em>x</em>) = 0<em>, etc.; remember that all you need to add a shape to your ray tracer are methods for ray intersection and computing normals.</em>

1

<strong>Problem 2 </strong>(15 points)<strong>. </strong><em>Right now our output looks pretty boring since there is no color and all the textures are Lambertian. Add support for Phong shading as discussed in the last assignment, and make sure each shape can have its own unique colored material.</em>

<strong>Problem 3 </strong>(15 points)<strong>. </strong><em>Add support for casting shadows.</em>

<strong>Problem 4 </strong>(15 points)<strong>. </strong><em>Add support for mirrored surfaces that reflect rays of light according to the law of reflection discussed in class. Be sure to limit recursion depth so that your ray tracer doesn’t get stuck!</em>

<strong>Problem 5 </strong>(15 points)<strong>. </strong><em>Use distribution ray tracing within each pixel to implement simple antialiasing.</em>

<strong>Problem 6 </strong>(25 points)<strong>. </strong><em>Include a short write-up of your ray tracer in a file entitled writeup.pdf. This write-up should include at least three images produced by your ray tracer demonstrating the features you have added.</em>

<strong>Problem 7 </strong>(Up to 15 points extra credit)<strong>. </strong><em>Add additional features to your ray tracer; be sure to discuss them in writeup.pdf and have them clearly labeled as extra credit. You’re welcome to come up with your own ideas; potential extensions include:</em>

<ul>

 <li><em>More complex materials</em></li>

 <li><em>Multiple lights or different light shapes</em></li>

 <li><em>Another application of distribution ray tracing as discussed in class</em></li>

 <li><em>Instancing</em></li>

 <li><em>Distance-based falloff attenuating lighting based on how far it has traveled</em></li>

 <li><em>Refractive surfaces, lenses</em></li>

 <li><em>Interesting shapes, CSG</em></li>

 <li><em>Acceleration techniques</em></li>

</ul>

<em>The best ray-traced final images will be shown in class.</em>

2