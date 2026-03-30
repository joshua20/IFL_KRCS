# IFL_KRCS

#to update county and subcounty boundaries

python manage.py load_boundaries --counties counties/ke_admin2.shp
python manage.py load_boundaries --subcounties subcounties/ke_subcounty.shp

#Migrate migrations
 docker exec -it krcs_backend python manage.py migrate
