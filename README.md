# React Accordion List
An accordion that was created with css and React. Use it in your projects. 

## How to Use

Pass a string (this.props.title) to give the accordion a title and an object (this.props.description) in the following format to populate the lines of the accordion

```javascript
//title 
let titleToBePassed = "Title of the Accordion";

//description
let descriptionToBePassed = { item1 : { 
                              name : "ITEM 1", 
                              link : "https//link.com"
                            },
                    item2 : { 
                              name : "ITEM 2"
                            }
                  };
                  
//Main App                  
class App extends Component {

    render() {
        return (
            <div className="App">
                <!-- Font Awesome CDN -->
                <link rel="stylesheet" 
                href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" 
                integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ" 
                crossOrigin="anonymous"  />
                <!-- Accordion Component -->
                <Accordion title={titleToBePassed} description={descriptionToBePassed} />
            </div>
        );
    }

```

Item 1 will have an anchor with a href of https//link.com while item 2 will be an empty button with no href.
