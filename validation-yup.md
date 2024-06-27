# Yup framework in validation

- basic manual validaiton

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
