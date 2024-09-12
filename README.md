Superheroes API
This project implements an API for managing superheroes and their powers using Flask, SQLAlchemy, and Flask-Migrate. The data model consists of three main entities: Hero, Power, and HeroPower, which are interconnected through relationships as outlined in the provided Entity Relationship (ER) Diagram.

Features
Heroes can have multiple powers and vice versa through a many-to-many relationship.
A HeroPower model connects Hero and Power with additional attributes such as strength.
Validations ensure data integrity, such as enforcing specific values for HeroPower and ensuring proper descriptions for Power.
API routes to create, retrieve, update, and delete resources for Hero, Power, and HeroPower.
Migrations and seeding are provided for database setup.
Models
The main models used in the API are:

Hero
Represents a superhero with a name and a unique identity.

Power
Represents a power that a hero can have, with a description of its effects.

HeroPower
A join model representing the many-to-many relationship between Hero and Power. It includes the following additional attributes:

strength: A string representing the intensity of a hero's power (e.g., 'Strong', 'Weak', 'Average').
Prerequisites
Python 3.9+
Flask
Flask-SQLAlchemy
Flask-Migrate
SQLite (or your preferred SQL database)
