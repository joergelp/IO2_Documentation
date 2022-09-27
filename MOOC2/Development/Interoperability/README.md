<p align="right">
  <a href="README.md">[EN]</a>
  <a href="README_es.md">[ES]</a>
  <a href="README_pt.md">[PT]</a>
  <a href="README_tr.md">[TR]</a>
  <a href="README_sv.md">[SV]</a>
</p>

# Interoperability

JuezLTI uses version 1.0 of the Learning Tools Interoperability standard (LTI) for integration into the LMS. 
This interoperability standard was proposed by the IMS Global Learning Consortium \cite{lti2010} 
and is supported by reference LMS vendors such as Moodle, Canvas, or Sakai.

With LTI a set of educational services can be used to extend the functionality of the LMS using a Service Oriented Architecture (SOA). 
The LMS becomes a marketplace where the teacher can select the resources from different providers to improve the learning experience. 

JuezLTI is based on TSUGI, a framework that simplifies the development and deployment of LTI applications. 
The first application of TSUGI was a self-contained MOOC for training in Python -- py4e.com. 
It was deployed by one of its authors, Dr. Charles Severance, founder of the Open Source LMS Sakai and currently working for IMS. 
LTI has been widely used since 2010, not only for code testing purposes 
but also for providing complex assessments not directly supported by the LMS, such as Dig4E, a tool to learn about standards for 
creating high-quality digital still images. 

To use JuezLTI the teacher has to request a  key/secret pair on the project's website. 
With those credentials and the supplied URL, the teacher adds an external activity in the LMS. 
The students are directly identified in JuezLTI using the information provided by the LMS. 
Whenever a student or teacher opens the activity, the LMS communicates with JuezLTI using LTI (via the TSUGI framework)
to identify the user and present the appropriate interface. Then, the LMS sends the <code>resource_link_id</code> property identifying the relevant activity. 
This way,  different activities can be added using the same key. Finally, JuezLTI reports grades of solved exercises back to the LMS using an LTI service. 

In short, there is bidirectional communication between JuezLTI and the LMS. 
JuezLTI stores the information of students and their results and sends the grades obtained back to the LMS. 
