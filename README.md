# django-bulma.io-template-mixins
Django template mixins for css framework bulma.io

Just a collection of useful example templates for bulma.io.

Form-mixins can be used with:  
`{% include 'form-mixins/form.html' %}` or `{% include 'form-mixins/form_card.html' %}`  
`with` optional parameters:  
- `form=my_form` set the form instance
- `form_url=my_form_url` set the url the form submits data to
- `form_method=post|get` form submit method
- `form_horizontal=True` if you want input labels on the same line as the input. Don't use paramater if you want label above input
- `no_button=True` if you want to place your own submit button. Else an "OK" button is automatically inserted

Furthermore in your form class you can add buttons:
```
class MyForm(forms.Form):
  buttons = {'Button name': 'button_type'} 
```
Where button type can be `submit`, `reset` , ...
