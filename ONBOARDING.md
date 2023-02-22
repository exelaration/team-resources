# Countries and States

Your wrap-up exercise for your onboarding is to make a website (can be just a single HTML page) that will use JavaScript to get data from an external REST API.  The details are as follows:

1. When the page loads, populate a dropdown menu with the results from a `GET` call to `https://xc-countries-api.fly.dev/api/countries/`
2. When a country is selected from the country dropdown, populate a second dropdown with the results from a `GET` call to `https://xc-countries-api.fly.dev/api/countries/<country_code>/states/`
3. Once all of that is done, create a way to add a new country by sending a `POST` call to `https://xc-countries-api.fly.dev/api/countries/`
5. Create a way to add new states by sending a `POST` call to `https://xc-countries-api.fly.dev/api/states/`

[Insomnia](https://insomnia.rest) and [Postman](https://www.postman.com) are tools for interacting with REST APIs (which is what `https://xc-countries-api.fly.dev/api/` is), so feel free to use them to experiment and understand the data your page will be receiving from the `GET` requests, and what it should send in a `POST` request.


## Troubleshooting

If you are have problems reaching the server API with your code,
and you want to check that the server is up vs your code having problems,
try loading
[https://xc-countries-api.fly.dev/api/countries/](https://xc-countries-api.fly.dev/api/countries/)
in your browser
and your browser should show you a JSON blob with country data.
If it does not, please contact someone in the onboarding Slack channel. 


## Stretch Goals
You may be referred to these activities by your mentor after completing the standard behavior described above. They are intended to increase your experience and understanding of a particular technology stack.


#### React Frontend:
 - Same behavior as the standard frontend, but written in ReactJS with reusable components. 
 - Dropdown behavior can be shared for Countries and States and configured via props.
 - A good primer on `bind` in JavaScript and it's use in ReactJS: [Explaining why we bind things in React](https://gist.github.com/fongandrew/f28245920a41788e084d77877e65f22f)

#### Django backend:
 - Create a backend in Django that works with either Frontend
 - Behavior should match the heroku endpoint, so the frontend code should only have to change to use a new base URL (get countries and get states for a country)


#### Django REST Framework Backend:
 - Adapt the Django backend to [Django REST Framework](https://www.django-rest-framework.org/) using Serializers and APIView
