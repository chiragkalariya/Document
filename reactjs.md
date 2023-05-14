1) What is component?
- A peace of code that can reuse
- such as Function
- but more powerfull then function
- ex. Header / Footer / and many section(component) use many time

2) Type of component?
- Function component
- Class component
- etc..

3) How to create Function component?
function User() {
    return(
        <>
            <h1>User component</h1>
        </>
    )
}
export default User;  

- import like this :
import user from './file path'
=======================================
- also you can use like this 
export function User() {
    return(
        <>
            <h1>User component</h1>
        </>
    )
}

- import like this :
import {user} from './file path'

4) Can we use component in another component?
- Yes you can use but you can't use outof component
- import User from './file path'
    function App() {
        function Apple() {
            return(
                <>
                    <div>apple component</div>
                </>
            )
        }
        return(
            <>
                <h1>Hello Workld</h1>
                {Apple()}  // show like this apple component
                <Apple />  // also you use like this
            </>
        )
    }

    export default App;

5) How to create class component?
- create User.js file // use first latter capital better standered
- 
    import React from 'react'
    class User extends React.Componetnt {

    }  // use any one

    import React,{Component} from 'react'
    class User extends Component {
        render() {
            return(
                <>
                    <h1>Hello from user</h1>
                </>
            )
        }
    }  // use any one

    export default User;

- import in another component
    import User from './file path'
    function App() {
        return(
            <>
                <h1>Hello Workld</h1>
                <User />  // show hear import component
            </>
        )
    }

    export default App;

6) Can we use ractjs and Angularjs in one project?
- Yes becaue, react is javascript library so you can use anyweare(in vuejs, angularjs)

7) Can I use JSX without reactjs?
- yes

8) Use of Click event & Function : 
-
    -- <button onClick={function()}>Click me</button>  // you are call function like this function will call on load page without click function
    -- <button onClick={function}>Click me</button>  // If you use without rounbrecate function will work properly
    -- If you want to use perameter so you can , use arrow function
        <button onClick={() => function(a)}>

9) Use of state in Functional Component : 
- state is object use for store data
- Use state is hook use for maintain state

- const [state, setState] = useState(initialState);

10) Use of state in Class component
- 

11) What is props?
- React components use props to communicate with each other. 
- Every parent component can pass some information to its child components by giving them props. 
- Props might remind you of HTML attributes, but you can pass any JavaScript value through them,
  including objects, arrays, and functions.

12) Props with functional component
- 

13) Props with class component
- 

14) Constructor life cycle method use in class component
- 

15) when use render method?
- reder use for data represent
- when component create
- when update state
- when update props

16) Life cycle method :
- componentDidMount
- componentDidUpdate(prevProps, prevState, snapShot)
- shouldComponentUpdate
- componentWillUnmount

17) Hooks
- Hooks is use for class component fetures use in function component feture
- Hooks
    -- useState
    -- useEffect // useEffect is callback function
    -- useMemo
    -- useRef  // useRef is use for DOM menipulate
    -- useParams
    -- useContext

18) Handle Array with list
    -- Array listing with map function

19) List with bootstrap and unique key
-- Nested list in table

20) Reuse component in loop

21) what is fragment?
- petern for handle multiple elements and component
- sign of fragment <></>
- types of use
    -- <React.fragment></React.fragment>
    -- import fragmetn from 'react'
        <fragment></fragment>
    -- <></>

22) pure component
- pure component is react feature that import from react
- pure component has stop component's re-rendering

23) Ref
- Ref only use in emargency 
- using ref modify DOM
- using in same component 

24) forwardRef 
- forwardref is advanced version of Ref
- using forwardref we can modify parent component and child component

25) controlled component
- in react controle inpute filed using state is control component
    uncontrol component : 
    -- directly control through DOM
    -- this can not control through stack

26) High order component (HOC) : 
- 

27) React Router : 
- react install using cmd : 
    -- npm i react-router-dom
- react uninstall using cmd :
    -- npm uninstall react-router-dom
- Navigate :
    -- using navigate redirect page one to another page(ex : Home page)   
- Dynamic Routing : 
    -- useParams Hooks             
- Nested Routing
    -- 
- Use Location
- Protected Router                                 

28) install react bootstrap : 
- npm install react-bootstrap bootstrap
- set path in index.js
    -- import 'bootstrap/dist/css/bootstrap.min.css'

29) Previous State in function Component : 
-  

30) Previous Props with Hooks :
- 

31) State with Object :
- use state with object

32) Context API : 
- Context API allows you to easily access data at different levels of the component tree,
without passing props to every level
steps : 
- createContext // create context
- provider 
- consumer // for consume data

33) Redux : 
- Redux is pattern and library  for managing and updating application state, using event called "action"
- A container where you can store your whole application data

-- Action  // collect data from API or component
-- Reducer  // get data from action and send to store
-- Store  // store is store state(Data) of complete Application
-- View  // view anywhere data from store

- install redux
-- npm i redux
-- npm i react-redux

------------------------------------------------------------------
-------------- Action.js -----------------------------------------



34) props drilling : 
- pass data child to one by one using props


35) Git setup : 
- install git 
- $ git config --global user.name "John Doe"
- $ git config --global user.email johndoe@example.com
- checking your setting :
- $ git config --list   // unnecessary
- $ ssh-keygen 
- after enter one time
- add padssword // two time
- open windows powershell
- $ Get-Content ~/.ssh/id_rsa.pub | Set-Clipboard   // past in window powershell 
(password was copy in your clip bord)
- open gitbash - setting - sshkey and add
- $ git add   // add file modifile and git new create file
- $ git commit -m "comment pass what to do ?"

- $ git push -u origin main

36) AXIOS :
- Axios allows us to communicate with APIs easily in our React apps.
- Axios is a promise-based library used with Node.

37) skelton loading :
- npm i react-loading-skeleton

