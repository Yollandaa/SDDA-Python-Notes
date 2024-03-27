# Flask and Databases
- type="Submit" triggers the action in the form.
- GET in a form -> exposes the user details in the url -> if it not sensitive information we can use it.
- use request.form.args() -> When the form is a GET.

## Connecting the db to Flask
- All the SQL queries we write they go directly to AZURE.
- We need a driver to connect Flask and Azure
    - Convert python to understandable SQL queries
    - If you just using the driver, you write RAW SQL -> "SELECT * movies" -> The data that comes back is difficult to use
    - SQL Alchemy -> Package ORM (Object Relation Mapping) -> To understand the data we receive from SQL -> Abstraction -> No RAW SQL. -> Auto-complete
        - Easy to work with datatypes -> can convert from class object to dict.
        - Auto complete -> .query (those all)
        - Can work with multiple databases. (Talks with MySQL, SQLServer, Postgres) -> Only change the connection string
    - 
- We do not need an __init__ in the class cuz it inherits from db.Model
- The .env won't be available to another person -> so privately send it to the other person.

    
## For DELETE
<form action="{{url_for('delete_movie_by_id')}}" method="POST">
            <input name="movie_id" type="text" value="{{movie.id}}" hidden />
            <button type="submit">Delete</button>
          </form>

@app.route("/movie-list/delete", methods=["POST"])  # HOF
def delete_movie_by_id():
    print(request.form.get("movie_id"))
    return "<h1>Movie deleted Successfully</h1>"

## Mentor Session
- Pespective on how customers interact with Sanlam
- Things I wanna learn: Could be about the business
- What I want to get out of this relationship.