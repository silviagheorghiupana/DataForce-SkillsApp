# DataForce-SkillsApp

Technologies:

FrontEnd : React JS
Backend : Python
Database: MongoDb
Arhitecture: Microservicii ( Admin, Members, Login, Projects, Ratings, Notifications)
Deploy : AWS :  EC2, ELB, Code Build, Code Deploy, EKS

Data Modelling
1. What we will store?
employees CVs: contact data, job history, skills, levels for skills, university and courses, certifications, personal projects, discipline, level and seniority in company, feedback/recommandation from clients, desired tech stack, desired carrer path,  desired job positions, desired industry, rates
2.How the data will be queried?
 Who is using the application and how?
 users (different roles) : project delivery managers
                           IT consultants
                           Hr 
                           carrer managers
                           clients
                           admin 
 project delivery managers => se logheaza => introduce proiect sau alege unul existent => cauta skilluri (tech name, framework is needed, seniority level, range for rating) => obtine informatii (a list of potential candidates with minimal display info, with some ordering) => for a specific candidat, get full details => create meeting invite for the candidate
 
 IT consultant => se logheaza => completeaza/incarca/updateaza datele despre el (orice ??? NU ) => search for availabl projects ( tech name, framework, seniority, industria) => obtine informatii ( a list of posible projects with basic details) => for a specific, get full details => request for info to the delivery manager
 
 Carrer Manager => se logheaza => listare subordonati => pentru un subordonat , vizualizare progress ( history of feedback , technology + rating ) => trimtie recomndare de cursuri => ii schimba nivelul de seniorutate => seteaza meetinguri 1-1 => rating (techologies, domains, soft skills)
 
 Hr => se logheaza => introduce/importa din HR system datele intiale , contact, job history => upadateaza statusul anagajati ( acitiv/inactiv) si soft skills
 
 Client => se logheaza (userul este generat la momentul crearii proiectului si trimis la clinet, ceva generic) => ii apar consultanti acitiv pe proiectele lui => alege unul => da rating (techologies, domains, soft skills)
 
 
                           
 
