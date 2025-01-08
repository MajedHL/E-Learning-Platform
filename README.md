# E-Learning-Platform
## Description
An online platform for learning.
- Admins:
  - Admins can create courses on the platform.
  - A course can include a combination of texts, images, and videos.
  - Admins can also create quizzes to evaluate students.
- Students:
  - Students can enroll in open courses, complete them, and take quizzes.
- Guest users:
  - Guest users can view the available courses and their descriptions.
  - However, they cannot access course details until they register and enroll.

## Repository structure
```
/super-repo
├── /backend-submodule (points to the backend repository)
├── /frontend-submodule (points to the frontend repository)
├── .gitmodules
└── README.md
```



## Clone
The backend and frontend of the application are added as submodules in this super repository.    
To clone the repository with its submodules run this command:
```bash
git clone --recurse-submodules https://github.com/MajedHL/E-Learning-Platform.git
```
To initialize submodules that haven't been initialized yet:
```
cd E-Learning-Platform/
git submodule update --init --recursive
```

To update the submodules to the latest commit from their remote repository run this command:
```
git submodule update --remote
```
To pull the latest changes from the super repository and update all submodules to the specific commits they are pointing to in the super repository.:
```
git pull --recurse-submodules
```
