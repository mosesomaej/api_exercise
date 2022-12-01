pip install fastapi fastapi-sqlalchemy pydantic alembic psycopg2 uvicorn python-dotenv

alembic init alembic

docker-compose build docker-compose up -----(1)

docker-compose run app alembic revision --autogenerate -m "New Migration" -------(2)

docker-compose run app alembic upgrade head #commit migration to the database ------(3)


Libraries

fastapi - framework
sqlalchemy - help manage database
pydantic
alembic - easily made migration from model and create table in the databse
psycopg2 - communication with database
uvicorn - server
python-dotenv - help load environment variables

initialize alembic -- alembic init alembic

create and connect database before start-up event