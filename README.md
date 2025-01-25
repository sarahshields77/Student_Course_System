template at stage where protected routes have been added and login form at [localhost:5173/login](http://localhost:5173/login)
.env needs to be added in backend - find in C: copy of assign 1
change line 15 in server.js (cors) to: app.use(cors({ credentials: true, origin: 'http://localhost:5173' }));
LoginForm.jsx - add: import { useNavigate } from 'react-router-dom';
const navigate = useNavigate();  in LoginForm()
and // redirect to the dashboard
            navigate('/dashboard');
in the handleSubmit try block
