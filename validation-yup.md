# Yup framework in validation
`import * as Yup from 'yup';`
- basic manual validaiton
      - set up form with disabled default, add an error useState in the code, use `helperText`, `error` and `onChange` to validate
      - model
                  ```
                    const validationSchema = Yup.object().shape({
                           x : Yup.string(),
                          ...
                        });
                  ```
      - validate function
              ```
                     const validateField = (field, value) => {
                          try {
                              validationSchema.validateSyncAt(field, { [field]: value });
                              setErrors(prevErrors => ({ ...prevErrors, [field]: '' }));
                          } catch (validationError) {
                              setErrors(prevErrors => ({ ...prevErrors, [field]: validationError.message }));
                          }
                      };
              ```
        - in HTML
              ```
                  validateField('x', e.target.value);
                  error={!!errors.x}
                  helperText={errors.x}
              ```
- datatype
- 
- disable basic HTML form `<form onSubmit={(event)=>{event.preventDefault();}} className="w100 h100">`
- start and end date

      yup.object({
        start: yup.date(),
        end: yup.date().min(yup.ref('start'))
      });

- can also work with framik 

- sql injection

        getKeyValues = (props, obj) => {        
        const escRegex = /\b(ALTER|CREATE|DELETE|DROP|EXEC(UTE){0,1}|INSERT( +INTO){0,1}|MERGE|SELECT|UPDATE|UNION( +ALL){0,1})\b/;
        props.forEach((el) => {
            if (obj.hasOwnProperty(el) && obj[el].search(escRegex)) obj[el] = '';
        })
        return obj;
    }

- 
