## :palm_tree: COVID-19 DASHBOARD Django Plotly Dash App

* [COVID-19 DASHBOARD Django Plotly Dash App](https://github.com/mazqoty/Dashbaord-Covid19-Django-Plotly_Dash)
  This COVID-19 Dashboard tracks covid-19 confirmed, deaths, recovered, active cases. It also contains vaccination analysis. The data was collected from various sources such as [CSSE at Johns Hopkins University](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series) and [Our World in Data](https://github.com/owid/covid-19-data/tree/master/public/data/vaccinations). This dashboard is made only for educational purpose.

<table style="width:100%">
  
  <tr>
    <td><img src="https://i.imgur.com/PwV2BEO.png" width="800px" height=400px/></td>
  </tr>
  <tr>
    <td><img src="https://i.imgur.com/93Y0Rrv.png" width="800px" height=400px/></td>
  </tr>
  <tr>
    <td><img src="https://i.imgur.com/ZPPIB5C.png" width="800px" height=400px/></td>
  </tr>
  <tr>
    <td><img src="https://i.imgur.com/zQICMOE.gif" width="800px" height=400px/></td>
  </tr>
</table>

### Usage

git clone https://github.com/mazqoty/Dashbaord-Covid19-Django-Plotly_Dash.git

go to the project folder and run vscode: `code .`

Create a virtual environment: `python -m venv venv` 

Activate the virtual environment: `source venv/bin/activate` or `venv/Scripts/activate.bat` 

Install Dependencies: `pip install -r requirements.txt` 

Change Directory: `cd app` 

Migrate the database: `python manage.py makemigrations`

Minimize the database: `python manage.py migrate`

Collect static files: `python manage.py collectstatic` 

Run the app: `python manage.py runserver`

Docker:

add `uWSGI>=2.0.18,<2.1` in `requirements.txt`

in `settings.py` change neccessary settings for SECRET_KEY, DEBUG, ALLOWED_HOSTS and Static files. See settings.py file

Run services in the background: `docker-compose up -d`

Run services in the foreground: `docker-compose up --build`

Copy and paste http://127.0.0.1:8000/ in the browser

Inspect volume: `docker volume ls` and `docker volume inspect <volume name>`

View networks: `docker network ls`

Bring services down: `docker-compose down`
