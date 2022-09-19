# The LTI Standard


The IMS Learning Tools Interoperability (LTI) specification can be defined as a standardized way to integrate third-party content into courses within an LMS or platform. Without LTI, LMS and content providers would have to rely on custom integrations with prejudice to interoperability and scalability.
This specification evolved from a simple mechanism to launch web applications
from the LMS, to support multiple services to securely interchange data with these applications. 
LTI is a standard supported by all LMS vendors of reference, and thus maximizes the
payoff of adapting an educational web application.


Nowadays, the IMS consortium recommends the adoption of version 1.3. In short, LTI 1.3 uses OAuth2 and signed messages using JSON Web Tokens (JWTs) to securely authenticate students and pass data between the LMS and the external learning tool. 

This version includes LTI Advantage, defined as a package of services that add new features to enhance the integration of any tool with any LMS in the core of LTI 1.3. The three LTI Advantage feature services are Names and Role Provisioning Services, Deep Linking, and Assignment and Grade Services:
 - Names and Role Provisioning Services (NRPS): grants the tool access to the list of users and their roles for a specific context (e.g. a course or group). NRPS allows the external tool to request a list of members from the context that launched it. Once the tool receives the membership list, it can read all students and teachers enrolled in the context, even if they have not yet launched the tool. 
 - Assignment and Grade Services (AGS): allows teachers to sync grades between third-party tools and their LMS. This service returns numeric scores and teacher comments to an LMS gradebook. For instance, a teacher can view when a student has started an assignment, or if it has been completed. The teacher can also receive the status of a grade, even if it requires manual input from the teacher.
 - Deep Linking (DL): offers a more streamlined approach to adding LTI links to an LMS. Deep Linking messages allow external learning tools to appear within an LMS as internal tools would. With Deep Linking, external learning tools can now allow teachers to configure specific content or activities within the tool. In LTI 1.1, the whole tool content had to be exposed, even if the teacher only wanted the class to use a specific resource. Deep Linking allows teachers to select whichever content they need and share the link to launch that content with their course. For example, a tool may let a teacher configure a specific chapter from an e-book when their students select a link, rather than force them to launch the tool and then navigate to that chapter.
    
Adopting LTI 1.3 should be a careful decision. For most of the cases, LTI 1.1 is enough in use cases where a student launches an activity from the LMS, solves it in the external tool and then a grade is reported back to the LMS grade book. However, the new LTI 1.3 features could be applied in relevant use-cases. For instance, considering the use of leaderboards: names and roles obtained from provisioning services could be used to populate leaderboards with the names of students before they submitted for the first time; deep links could be used to embed in LMS content leaderboards generated on-the-fly by the tool.


## Choice of language
- [English](README.md)
- [Spanish](README_es.md)
- [Portuguese](README_pt.md)
- [Swedish](README_sv.md)
- [Turkish](README_tr.md)
