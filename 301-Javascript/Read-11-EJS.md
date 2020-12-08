# READ-11-EJS

### What is EJS?

- EJS or Embedded Javascript Templating is a simple templating language that lets you generate HTML markup with plain JavaScript.

### Getting Started.

- Create instance of the server.
- `var app = express();`

- Configure Express to run everything through body parser and cors.
- `app.use(bodyParser());`
- `app.use(cors());`

- set the views folder to handle all of the views being created.
- `app.set('views', path.join(dirname, 'views'));`

- Create view engine set that to EJS.
- `app.set('view engine', 'ejs');`

### Evaluate an Injected variable.
- `app.get('/', function (req,res) {
    response.render('index', {
      foo: 'bar'
    });
});`

html-index.ejs

`<h1> <%= foo %></h1>` === `<h1> bar</h1>`


### Loop over an array of values.
- `app.get('/', function (req,res) {
    response.render('index', {
      person: [
        {name:'dave'},
        {name:'jerry'}
        ]
    });
});`

html-index.ejs

<ul>
<% for(var person of people) { %>
<li><%person.name%></li>
<% } %>
</ul>

### If/else statements.

<ul>
<% for(var person of people) { %>
  <%if(person.name === 'dave') { %>
  <li>This is definatley <%person.name%>!</li>
  <% } %>
<% } %>
</ul>

### Layouts

### Portfolios



