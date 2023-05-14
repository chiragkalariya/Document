3)What is the children prop?
a property that lets you pass data to child elements

4) We can update the state in React.js by calling to setState() method. These calls are:
B. Asynchronous in nature

6) Which attribute do you use to replace innerHTML in the browser DOM?
B. dangerouslySetInnerHTML

7) Difference between State and Props
- State only use in component
- props passed to another component
- state use for a display changes
- props use for pass data between components, use props to communicate with each other.
- state use in function component using useStat hook
- and state use in class component this.state
- props can use in function component using perameter
- props can use in class component using this.props

8) Write Code for API call with AXIOS And Create Page of Blog Cards

import React, { useEffect, useState } from 'react'

const FetchApiData = () => {
    const [data, setData] = useState([]);
    useEffect(() => {
        fetch("https://jsonplaceholder.typicode.com/posts").then((result) => {
            result.json().then((resp) => {
                setData(resp);
            })
        })
    })
    return (
        <div className='card_main' style={{display: "grid", gridTemplateColumns: "auto auto auto auto", gap: "15px", padding: "50px", textAlign: "left"}}>
            {
                data.map((i) =>
                    <div className="card" style={{padding: "50px 15px"}}>
                        <code>{i.id}</code>
                        <h4 style={{marginBottom: "1rem"}}>{i.title}</h4>
                        <p>{i.body}</p>
                    </div>
                )
            }
        </div>
}
export default FetchApiData;


9) Write Code for API call with AXIOS And Create Page of Blog Cards

const FetchApiData = () => {
    useEffect(() => {
        fetch("https://jsonplaceholder.typicode.com/comments").then((result) => {
            result.json().then((resp) => {
                console.log(resp);
            })
        })
    })
    return (
        <>
            
        </>
    )
}
export default FetchApiData;

