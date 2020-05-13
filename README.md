# Responsive web design


- Responsive web design is about creating web pages that look good on all devices!

         <html>
         <head>
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
         </head>
    
      
      
-  A responsive web design will automatically adjust for different screen sizes and viewports.

- This will set the viewport of your page, which will give the browser instructions on how to control the page's dimensions and scaling.





# Flexible Box:
- The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

- To start using the Flexbox model, you need to first define a *flex container*.
#### Parent Element (Container):

* The flex container becomes flexible by setting the display property to flex:
    
    
        .flex-container {
          display: flex;
           }
 
## The flex container properties :
   1. flex-direction 
   2. flex-wrap
   3. flex-flow
   4. justify-content
   5. align-items
   6. align-content
   
### flex-direction property:
     
* The flex-direction property defines in which direction the container wants to stack the flex items.

**Example**
* The column value stacks the flex items vertically (from top to bottom):

              <!DOCTYPE html>
              <html>
              <head>
              <style>
              .flex-container {
                display: flex;
                flex-direction: column;
                background-color: DodgerBlue;
              }

              .flex-container > div {
                background-color: #f1f1f1;
                width: 100px;
                margin: 10px;
                text-align: center;
                line-height: 75px;
                font-size: 30px;
              }
              </style>
              </head>
              <body>
              <h1>The flex-direction Property</h1>

              <p>The "flex-direction: column;" stacks the flex items vertically (from top to bottom):</p>

              <div class="flex-container">
                <div>1</div>
                <div>2</div>
                <div>3</div>  
              </div>

              </body>
              </html>


### The flex-wrap Property:
* The flex-wrap property specifies whether the flex items should wrap or not.


* The examples below have 12 flex items, to better demonstrate the flex-wrap property.

        <!DOCTYPE html>
        <html>
        <head>
        <style>
        .flex-container {
          display: flex;
          flex-wrap: wrap;
          background-color: DodgerBlue;
        }

        .flex-container > div {
          background-color: #f1f1f1;
          width: 100px;
          margin: 10px;
          text-align: center;
          line-height: 75px;
          font-size: 30px;
        }
        </style>
        </head>
        <body>
        <h1>The flex-wrap Property</h1>

        <p>The "flex-wrap: wrap;" specifies that the flex items will wrap if necessary:</p>

        <div class="flex-container">
          <div>1</div>
          <div>2</div>
          <div>3</div>  
          <div>4</div>
          <div>5</div>
          <div>6</div>  
          <div>7</div>
          <div>8</div>
          <div>9</div>  
          <div>10</div>
          <div>11</div>
          <div>12</div>  
        </div>

        <p>Try resizing the browser window.</p>

        </body>
        </html>
          
## The flex-flow Property:

* The flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.

> * Example 

          <!DOCTYPE html>
          <html>
          <head>
          <style>
          .flex-container {
            display: flex;
            flex-flow: row wrap;
            background-color: DodgerBlue;
          }

          .flex-container > div {
            background-color: #f1f1f1;
            width: 100px;
            margin: 10px;
            text-align: center;
            line-height: 75px;
            font-size: 30px;
          }
          </style>
          </head>
          <body>
          <h1>The flex-flow Property</h1>

          <p>The flex-flow property is a shorthand property for the flex-direction and the flex-wrap properties.</p>

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div>3</div>  
            <div>4</div>
            <div>5</div>
            <div>6</div>  
            <div>7</div>
            <div>8</div>
            <div>9</div>  
            <div>10</div>
            <div>11</div>
            <div>12</div>  
          </div>

          <p>Try resizing the browser window.</p>

          </body>
          </html>


### The justify-content Property:

> The justify-content property is used to align the flex items:

* Example

> The center value aligns the flex items at the center of the container:


            <!DOCTYPE html>
            <html>
            <head>
            <style>
            .flex-container {
              display: flex;
              justify-content: center;
              background-color: DodgerBlue;
            }

            .flex-container > div {
              background-color: #f1f1f1;
              width: 100px;
              margin: 10px;
              text-align: center;
              line-height: 75px;
              font-size: 30px;
            }
            </style>
            </head>
            <body>
            <h1>The justify-content Property</h1>

            <p>The "justify-content: center;" aligns the flex items at the center of the container:</p>

            <div class="flex-container">
              <div>1</div>
              <div>2</div>
              <div>3</div>  
            </div>

            </body>
            </html>
            
            
### The align-items Property:

* The align-items property is used to align the flex items vertically.

* Example

> The center value aligns the flex items in the middle of the container:

          <!DOCTYPE html>
          <html>
          <head>
          <style>
          .flex-container {
            display: flex;
            height: 200px;
            align-items: center;
            background-color: DodgerBlue;
          }

          .flex-container > div {
            background-color: #f1f1f1;
            width: 100px;
            margin: 10px;
            text-align: center;
            line-height: 75px;
            font-size: 30px;
          }
          </style>
          </head>
          <body>
          <h1>The align-items Property</h1>

          <p>The "align-items: center;" aligns the flex items in the middle of the container:</p>

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div>3</div>  
          </div>

          </body>
          </html>
          
          
### The align-content Property:

* The align-content property is used to align the flex lines.

* Example: 

> The flex-start value displays the flex lines at the start of the container:

          <!DOCTYPE html>
          <html>
          <head>
          <style>
          .flex-container {
            display: flex;
            height: 600px;
            flex-wrap: wrap;
            align-content: flex-start;
            background-color: DodgerBlue;
          }

          .flex-container > div {
            background-color: #f1f1f1;
            width: 100px;
            margin: 10px;
            text-align: center;
            line-height: 75px;
            font-size: 30px;
          }
          </style>
          </head>
          <body>
          <h1>The align-content Property</h1>

          <p>The "align-content: flex-start;" displays the flex lines at the start of the container:</p>

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div>3</div>  
            <div>4</div>
            <div>5</div>
            <div>6</div>  
            <div>7</div>
            <div>8</div>
            <div>9</div>  
            <div>10</div>
            <div>11</div>
            <div>12</div>  
          </div>

          </body>
          </html>

- OutPut:

### Child Elements (Items):

* The direct child elements of a flex container automatically becomes flexible (flex) items.

          <!DOCTYPE html>
          <html>
          <head>
          <style>
          .flex-container {
            display: flex;
            background-color: #f1f1f1;
          }

          .flex-container > div {
            background-color: DodgerBlue;
            color: white;
            width: 100px;
            margin: 10px;
            text-align: center;
            line-height: 75px;
            font-size: 30px;
          }
          </style>
          </head>
          <body>

          <h1>Flexible Items</h1>

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div>3</div> 
            <div>4</div>
          </div>

          <p>All direct children of a flexible container becomes flexible items.</p>

          </body>
          </html>

### The flex item properties :
- order
- flex-grow
- flex-shrink
- flex-basis
- flex
- align-self

##### The order Property:

   - The order property specifies the order of the flex items.

              <!DOCTYPE html>
              <html>
              <head>
              <style>
              .flex-container {
                display: flex;
                align-items: stretch;
                background-color: #f1f1f1;
              }

              .flex-container>div {
                background-color: DodgerBlue;
                color: white;
                width: 100px;
                margin: 10px;
                text-align: center;
                line-height: 75px;
                font-size: 30px;
              }
              </style>
              </head>
              <body>
              <h1>The order Property</h1>

              <p>Use the order property to sort the flex items as you like:</p>

              <div class="flex-container">
                <div style="order: 3">1</div>
                <div style="order: 2">2</div>
                <div style="order: 4">3</div> 
                <div style="order: 1">4</div>
              </div>

              </body>
              </html>
              
              
- OutPut:

### The flex-grow Property:


- The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items.

        <div class="flex-container">
          <div style="flex-grow: 1">1</div>
          <div style="flex-grow: 1">2</div>
          <div style="flex-grow: 8">3</div>
        </div>
        
- Output:


### The flex-shrink Property:


- The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.

* Example

         <div class="flex-container">
          <div>1</div>
          <div>2</div>
          <div style="flex-shrink: 0">3</div>
          <div>4</div>
          <div>5</div>
          <div>6</div>
          <div>7</div>
          <div>8</div>
          <div>9</div>
          <div>10</div>
        </div>
       
- OutPut:


### The flex-basis Property :

- The flex-basis property specifies the initial length of a flex item.

* Example

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div style="flex-basis: 200px">3</div>
            <div>4</div>
          </div>

- OutPut :



### The flex Property:

- The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.

* Example :

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div style="flex: 0 0 200px">3</div>
            <div>4</div>
          </div>

- OutPut:

### The align-self Property:

- The align-self property specifies the alignment for the selected item inside the flexible container.

- The align-self property overrides the default alignment set by the container's align-items property.

* Example

      - Align the third flex item in the middle of the container:

          <div class="flex-container">
            <div>1</div>
            <div>2</div>
            <div style="align-self: center">3</div>
            <div>4</div>
          </div>

### CSS Media Queries :

#### What is a Media Query?
- Media query is a CSS technique introduced in CSS3.

- It uses the @media rule to include a block of CSS properties only if a certain condition is true.

* Example1 :


        <!DOCTYPE html>
        <html>
        <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
        body {
          background-color: yellow;
        }

        @media only screen and (max-width: 600px) {
          body {
            background-color: lightblue;
          }
        }
        </style>
        </head>
        <body>

        <p>Resize the browser window. When the width of this document is 600 pixels or less, the background-color is "lightblue", otherwise it is "lightgreen".</p>

        </body>
        </html>

- OutPut :
  
* Example2:

- The following example shows a menu that will float to the left of the page if the viewport is 480 pixels wide or wider (if the viewport is less than 480 pixels, the menu will be on top of the content):
       
       <!DOCTYPE html>
        <html>
        <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
        .wrapper {overflow: auto;}

        #main {margin-left: 4px;}

        #leftsidebar {
          float: none;
          width: auto;
        }

        #menulist {
          margin: 0;
          padding: 0;
        }

        .menuitem {
          background: #CDF0F6;
          border: 1px solid #d4d4d4;
          border-radius: 4px;
          list-style-type: none;
          margin: 4px;
          padding: 2px;
        }

        @media screen and (min-width: 480px) {
          #leftsidebar {width: 200px; float: left;}
          #main {margin-left: 216px;}
        }
        </style>
        </head>
        <body>

        <div class="wrapper">
          <div id="leftsidebar">
            <ul id="menulist">
              <li class="menuitem">Menu-item 1</li>
              <li class="menuitem">Menu-item 2</li>
              <li class="menuitem">Menu-item 3</li>
              <li class="menuitem">Menu-item 4</li>
              <li class="menuitem">Menu-item 5</li>
            </ul>
          </div>

          <div id="main">
            <h1>Resize the browser window to see the effect!</h1>
            <p>This example shows a menu that will float to the left of the page if the viewport is 480 pixels wide or wider. If the viewport is less than 480 pixels, the menu will be on top of the content.</p>
          </div>
        </div>

        </body>
        </html>
        
        
- OutPut img10:

###  various kinds of screen resolutions :

 - Laptops:
 
       - @media screen 
          and (min-device-width: 1200px) 
          and (max-device-width: 1600px) 
          and (-webkit-min-device-pixel-ratio: 1) { 
        }
        
        
   - Tablets :
        
                  @media only screen 
            and (min-device-width: 768px) 
            and (max-device-width: 1024px) 
            and (-webkit-min-device-pixel-ratio: 1) {

          }
          
          
   - Phones :
       
                 @media only screen 
            and (min-device-width: 320px) 
            and (max-device-width: 480px)
            and (-webkit-min-device-pixel-ratio: 2) {

          }
          
    - Watches :
    
                  @media
            (max-device-width: 42mm)
            and (min-device-width: 38mm) { 

          }



  
