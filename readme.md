# INTERN MANAGEMENT SYSTEM (IMS)
- An intern application and progress management portal
<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## About the project

- It will allow a student to apply for an attachment/internship, receive confirmation and record their progress all in one system.
- The school supervisor should also be able to pull his student's records to his email in a neat/pretty format
- The hr staff should be able to view and approve applications
- The work supervisor should comment/make remarks on a students progress.
- The system should generate a comprehensive report on all of these. (PDF & CSV)



## Main users
- Interns/Attaches
- School lecturers(supervisors)
- Work supervisor(boss)
- Human resource
- Super Administrator



## Student flow
- Interns get an "apply" view where they submit their CVs and required documents. (Into a DB)
- HR staff view the applications and approve the ones that make the cut and send email notifications with the register link. 
	- If one does not qualify they get a rejection email
- Student registers on the portal and proceeds to log in. (JUMP->Login Module)
- Student keys in weekly performance which is stored in a DB
- At the end of the internship, the administrator approves the student's progress and gives their remarks.
- Student prints report and submit it to school


## Boss flow

- Boss login (JUMP->Login module)
- Boss sees a dashboard with a list of all students in their department
- Boss clicks on one student and sees their progress and if complete, gives a remark.  
- Boss locks the student out of the portal to stop them from editing the results

## HR flow
- HR  login (JUMP->Login module)
- Views applications
- Approve/reject applications
- Send emails/message



## Super admin flow
- Admin  login (JUMP->Login module)
- See all interns/ attaches
- See all bosses
- See  all users of the system generally



## Access rights
- The project has been hosted on a private GitHub repository. Open [this link](https://github.com/lewis-munyi/IMS--Intern-Management-System-/invitations) to
 see if you have been invited to it.
 
- Contact the repo [owner](mailto:lewismunyi97@gmail.com) to request access if 
you still can't access it. 

## Contributing

- Create a separate branch from the [master branch](https://github.com/lewis-munyi/IMS--Intern-Management-System-/tree/master) (or any other branch), identified by your name. 

- All your commits should be pushed to this branch.

- Forks and pull requests are also welcome.
 
- **Do NOT make any commits to the master branch** 

- After completion of the project, all branches will be merged into one whole 
system on the master branch


## Communication

- If you want to raise any issue feel free to contact [Santana](mailto:santanamash@gmail.com) or
 [Alex (Boss)](mailto:asenaalex@gmail.com) directly or through the WhatsApp group 


# Technical details
- The system has been built using the [Laravel](https://laravel.com) framework, an open-sourced software licensed 
under the [MIT license](https://opensource.org/licenses/MIT).

## Requirements
- MAC users should check out tutorials on how to set up laravel from the official landing page.
- **PHP v7.1+** 
    - If you are on windows, install the latest version of [Xampp](https://www.apachefriends.org/download.html)
    or any other app.
    - If you are on Ubuntu use this [tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04)
     to learn how to set up LAMP on your PC. If you're a nerdy one, running any other distribution, chances are you already know how to do all these. :p
- **Mysql server**
    - See teh above instructions
- **Web server**
    - A web server like [apache](https://httpd.apache.org/) or [nginx](https://nginx.com)
    - See the previous instructions to learn how to
- **Composer**
    - Head over to [getcomposer](https://getcomposer.org) and download your version for windows
    - For ubuntu users, run ```sudo apt install composer``` to set it up on your pc
- **Git**
    - Windows - [Download](https://git-scm.com/downloads) and install  git 
    - Ubuntu - ```sudo apt install git```
- A verified [Github Account](https://github.com) account
- **[Node JS](https://nodejs.org)**
- A text editor/ide like [VS Code](https://code.visualstudio.com/)

## How to run tn the app
- Create a new database called ``IMS``
- Open terminal or command prompt on your pc
- ```git clone``` the repository onto your pc and ``cd`` into it
- run ```npm install```
- run ```composer install```
- Open the ```.env.example``` file and copy all its contents into a new file named ```.env ``` and store it at the root 
of the project
- Edit the ``APP_NAME`` variable and set it to ``APP_NAME=IMS``
- Set ``DB_DATABASE=IMS``
- Set ``DB_USERNAME=`` to your user mysql username and ``DB_PASSWORD=`` to your mysql password
- Run ``php artisan key:generate``
- Run ``php artisan migrate``
- Run ``php artisan serve`` You should see some ``Laravel development server started: <http://127.0.0.1:8000>``
- Open a new terminal window and run ``npm run watch``. It should compile successfully
- Navigate to [localhost:8000/](localhost:8000/) on your browser to see the app.

## Tutorials
Tutorials on how to tweak the app can be found free on [Laracasts](https://laracasts.com/series/laravel-from-scratch-2017)


  
