# Boostrap note
The most no-brainer framework in React


# React-Bootstrap `2.10.2`
## Component

### Form
Basic form and text
-     <Form.Label htmlFor="inputPassword5">Password</Form.Label>
        <Form.Control
          type="password"
          id="inputPassword5"
          aria-describedby="passwordHelpBlock"
        />
      <Form.Text id="passwordHelpBlock" muted>
        Your password must be 8-20 characters long, contain letters and numbers,
        and must not contain spaces, special characters, or emoji.
      </Form.Text>
   
Dropdown
-     <Form.Select aria-label="Default select example">
          <option>Open this select menu</option>
          <option value="1">One</option>
          <option value="2">Two</option>
          <option value="3">Three</option>
        </Form.Select>

Toggle Switch
-     <Form.Check // prettier-ignore
          type="switch"
          id="custom-switch"
          label="Check this switch"
        />

Floating Label
-     <FloatingLabel
        controlId="floatingInput"
        label="Email address"
        className="mb-3"
      >
        <Form.Control type="email" placeholder="name@example.com" />
      </FloatingLabel>
      <FloatingLabel controlId="floatingPassword" label="Password">
        <Form.Control type="password" placeholder="Password" />
      </FloatingLabel>

Validation
- built in   `required `

            const [validated, setValidated] = useState(false);
            const handleSubmit = (event) => {
            const form = event.currentTarget;
            if (form.checkValidity() === false) {
              event.preventDefault();
              event.stopPropagation();
            }
            setValidated(true);
            };
      
  
### Accordion


### Alerts


### Badges

### Buttons

### Cards
### Carousels
### Close Button
### Images
### List groups

### Modals
### Navs and tabs
### Offcanvas
### Placeholders
### Progress bars
### Spinners
### Tables
### Toasts


## Bootstrap css
Use `className` instead of css
### Border
- `border-top`, `border-right`, `border-bottom`, `border-left`
- `border-0` ...
- `border border-primary` ...
- `rounded`, `rounded-circle` ...

### Breakpoint
- `sm` : landscape phones, 576px and up
- `md` : Medium devices (tablets, 768px and up)
- `lg` : Large devices (desktops, 992px and up)
- `xl` : Extra large devices (large desktops, 1200px and up)

### Display parent
`d-{breakpoint}-{value}` for sm, md, lg, and xl.
- `none`          does not display
- `inline`        in one line
- `inline-block`  in one line and variable height
- `block`         take up 100% width
- `table`         
- `table-cell`
- `table-row`
- `flex`          flexible
- `inline-flex`   navbar

### Color
- `text-secondary` grey
- `.text-danger` red
- `text-warning` yellow
- `text-muted` light grey

### Flex
- `flex-column`
- `flex-column-reverse`
- -- center  parental
  - `justify-content-start`
  - `justify-content-end`
  - `justify-content-center`
  - `justify-content-between`
  - `justify-content-around`
- | center  parental
  - `align-items-start`
  - `align-items-end`
  - `align-items-center`
  - `align-items-baseline`
  - `align-items-stretch`
- self  children
- auto
  
### Float
- `float-left`, `float-right`, `float-none`

### Visible
- `visible`, `invisible`


### Position
- `position-static`, `position-relative`, `position-absolute`, `position-fixed`, `position-sticky`

### Size
- `w-25`, 50, 75, 100 : width
- `mw- `


### Spacing 
- `m, p` +
- `t, b, l, r, x, y` +
- `0 ~ 5 / auto`

### Text
- `text-left`, `text-center`, `text-right`
- `text-truncate`
- `text-lowercase`, `text-uppercase`, `text-capitalize`
- `font-weight-bold`, `font-italic`





# React General Trick
- Define colors in css variable
- Span is for incline and Div is for section




## Bootstrap Icon 
svg files
