## UiPath integrate with ServiceNow, Chatbot and Streamlit
The scenario of how we can use ServiceNow with UiPath. It can be used in fusion with RPA (Robotic Process Automation) to bring many business benefits like integrating heterogeneous platforms through unified workflows, and automatically resolving incidents and IT and non-IT requests.
![alt_text](https://github.com/bacdillon/RPA-UiPath/blob/main/ServiceNow%20Integration/img/1.jpg)

## Watch Alfred in Action - 1. CSM IT Service Request System 👇	
[![IMAGE ALT TEXT HERE](https://github.com/bacdillon/UiPath/blob/main/CRM%20Alfred%20Bot/img/Alfred%20Action.jpg)](https://youtu.be/7A28HLdXn0E)

## Watch Alfred in Action - 2 ServiceNow Incident 👇	
[![IMAGE ALT TEXT HERE](https://github.com/bacdillon/UiPath/blob/main/CRM%20Alfred%20Bot/img/Alfred%20Action.jpg)](https://youtu.be/dW5v2IagOM8)

## Chabot Integration 👇	
[![IMAGE ALT TEXT HERE](https://github.com/bacdillon/RPA-UiPath/blob/main/ServiceNow%20Integration/img/09.jpg)](https://bacdillon.github.io/Digital-IT-Helpdesk-Support/)

<!DOCTYPE html>
<html>
<head>
<style>
/* From Uiverse.io by mrhyddenn */ 
button {
    position: relative;
    margin: 0;
    padding: 0.8em 1em;
    outline: none;
    text-decoration: none;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    border: none;
    text-transform: uppercase;
    background-color: #333;
    border-radius: 10px;
    color: #fff;
    font-weight: 300;
    font-size: 18px;
    font-family: inherit;
    z-index: 0;
    overflow: hidden;
    transition: all 0.3s cubic-bezier(0.02, 0.01, 0.47, 1);
  }
  
  button:hover {
    animation: sh0 0.5s ease-in-out both;
  }
  
  @keyframes sh0 {
    0% {
      transform: rotate(0deg) translate3d(0, 0, 0);
    }
  
    25% {
      transform: rotate(7deg) translate3d(0, 0, 0);
    }
  
    50% {
      transform: rotate(-7deg) translate3d(0, 0, 0);
    }
  
    75% {
      transform: rotate(1deg) translate3d(0, 0, 0);
    }
  
    100% {
      transform: rotate(0deg) translate3d(0, 0, 0);
    }
  }
  
  button:hover span {
    animation: storm 0.7s ease-in-out both;
    animation-delay: 0.06s;
  }
  
  button::before,
  button::after {
    content: '';
    position: absolute;
    right: 0;
    bottom: 0;
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background: #fff;
    opacity: 0;
    transition: transform 0.15s cubic-bezier(0.02, 0.01, 0.47, 1), opacity 0.15s cubic-bezier(0.02, 0.01, 0.47, 1);
    z-index: -1;
    transform: translate(100%, -25%) translate3d(0, 0, 0);
  }
  
  button:hover::before,
  button:hover::after {
    opacity: 0.15;
    transition: transform 0.2s cubic-bezier(0.02, 0.01, 0.47, 1), opacity 0.2s cubic-bezier(0.02, 0.01, 0.47, 1);
  }
  
  button:hover::before {
    transform: translate3d(50%, 0, 0) scale(0.9);
  }
  
  button:hover::after {
    transform: translate(50%, 0) scale(1.1);
  }
  
  
</style>
</head>
<body>

    <button>
        <span>Hover me</span>
    </button>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
