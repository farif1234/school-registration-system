# Sharp Benders Academy Database

Web application to manage data for a school system. Allows an administrator to perform CRUD operations on students, majors, advisors, instructors, and more. Admin can also register students for courses and assign instructors to courses. Website front end created with Bootstrap. Back end created with Flask and MySQL. 

## Screenshots 
![students](https://user-images.githubusercontent.com/88285952/199621306-e4d769c7-d581-4bbf-b36d-7414b9ad996c.png) 
![image1](https://user-images.githubusercontent.com/88285952/199621713-f5af3072-6f57-4818-8111-9f72d6c371aa.png)
(sample data)

## Schema
![schema](https://user-images.githubusercontent.com/88285952/199621590-1f20faff-ad7e-4614-9e49-f5a710f34f6c.png)


## Getting started

- CD to directory on flip servers, then clone git repo
- Install python virtual environment module
```bash
pip3 install --user virtualenv
```
- Create virtual environment, then activate
```bash
python3 -m venv ./venv
```
```bash
source ./venv/bin/activate
```
- Install dependencies
```bash
pip3 install -r requirements.txt
```
- Create .env file in root directory with below credentials for database access
```text
340DBHOST=classmysql.engr.oregonstate.edu
340DBUSER=cs340_lastnamef
340DBPW=maybea4digitnumber
340DB=cs340_lastnamef
```
- Change port number on app.py
```python
if __name__ == "__main__":
    app.run(port=XXXX, debug=True)
```
- Run gunicorn (replacing XXXX with port number you chose)
```bash
gunicorn -b 0.0.0.0:XXXX -D app:app
```

## Citations*

**Homepage Rotator Images**
- (May 2022) The Last Airbender HD wallpaper, image source, https://www.wallpaperflare.com/avatar-digital-wallpaper-avatar-the-last-airbender-wallpaper-270453
- (May 2022) Avatar Cycle Wallpaper, image source, https://cutewallpaper.org/download.php?file=/22/avatar-cycle-wallpapers/2387024546.jpg
- (May 2022) Wallpaper Avatar the Last Airbender, image source, https://wallpaperforu.com/wallpaper-avatar-the-last-airbender/

**Edit & Delete Icons**
- (May 2022) pencil.svg, image source, https://design-system.w3.org/styles/svg-icons.html
- (May 2022) trash.svg, image source, https://design-system.w3.org/styles/svg-icons.html

**Website Templates (.j2 files)**
- (June 2022) Flask-Starter-App, template code resource, https://github.com/osu-cs340-ecampus/flask-starter-app/tree/master/bsg_people_app/templates

**Additional citations given within source code*
