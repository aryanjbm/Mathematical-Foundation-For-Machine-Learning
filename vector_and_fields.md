<h2>Core Idea</h2>
The Goal is to understand the fundamental building blocks used to repersent and manipulate data in machine learning <b> Vectors </b> the <b>Space</b> they live in and the <b> Fields</b> of numbers they are built from.


<h2> Vector: A Description of Something </h2>
A vector is simply an ordered list of numbers that repersents a single data point. Each number in the list is a feature or attribute of the data point.

<h3>Example: Patient Reacord</h3>
<ul>
  <li>We can repersent Patient_A record with the vector : [120,98,76,98]</li>
  <li>This Corresponds to the feature : [Blood Pressuew,Glucose Level,Heart Rate,Spo2 Level]</li>
  <li> The Vector is a single point in 4 dimenstional space </li>
</ul>


This is often called a <b>feature vector</b> this how we convert real-world concepts into a language computer can understand.



<h2> Vector Space: A Playground You Can't Escape </h2>
A vector space is "universe" or "playground" where all our vectors of certain type live. For a collection of vectors to be proper vector space , it must follow simple rules:
<ol>
  <li><b>Rule1:Closure Under Addition. </b> if you take any two vectors and add them together, the resulting vector is still inside the playground.
  <b>Example: All points in 2d space (1,2)+(2,3) = (3,5) </b>
  </li>
  <li><b>Rule2:Closure Under Scalar Multiplication </b> if you take any vector and "scale" it , the resulting vector is still inside the playground.
   <b>Example: All points in 2d space (1,2)*2 = (2,4) </b> </li>
</ol>

These two rules guranteed that when we combine or manipulate data in these basic ways, the result is still a valid and meaningful data point of same type.


<h2> Field: A well behaved rulebook for arithmetic. </h2>

For a set of numbers to be <b>Field</b>, it must support all the operation you're used to : addition , subtraction, multiplication and most importantly division.

<ul>
  <li><b>The Crucial Property: Multiplicative Inverse </b> every number in the field (except 0) must have an inverse . this is ehat makes division possible.
  <b> Ability to mutliply by inverse guarantees that our mathematical operation are reversible. </b>
  </li>
</ul>

These two rules guranteed that when we combine or manipulate data in these basic ways, the result is still a valid and meaningful data point of same type.
<table>
  <tr>
    <td>Set of Numbers</td>
    <td>Is it a Field?</td>
    <td>Intutive Reason</td>
  </tr>
  <tr>
    <td>Real  Numbers(R)</td>
    <td> Yes </td>
    <td> you can divide any real number by another real number (except 0) and the result is still a real number.</td>
  </tr>
  <tr>
    <td>Integers(Z)</td>
    <td> No </td>
    <td> 1/2 not in Z.</td>
  </tr>
  <tr>
    <td>Integers Modulo 5(Z<sub>5</sub>)</td>
    <td>Yes</td>
    <td>A surise ! With "clock arithemetic ," all operation incluing inverse , result in set {0,1,2,3,4}
    example 3/2 means 3*inv(2) to find (inv(2)*2) mod 5  =1 then inv(2)=3 bcz (3*2)%5=1 so (3/2) mod 5 = 3*3 mod 5 =  4
    </td>
    
  </tr>
</table>

<h2>Putting It All Together</h2>

We use numbers from well bheaved <b>Field(like all real numbers)</b> to construct <b>Vectors</b> that describe our data. These vectors all exist and ineract withing a structured <b> Vector Space.</b>







