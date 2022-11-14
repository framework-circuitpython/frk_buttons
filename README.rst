===========
frk_buttons
===========

This is a managed group of digital inputs generally used for pushbuttons but can be used for any grouped digital input devices. It is a light wrapper over the buttons CircutPython keypad core module. So far it only supports the Keys class.

Usage
-----

In your project conf.py file, include a Buttons driver.

.. code-block:: python
    
    # conf.py
    conf = {
        'buttons':
            {'driver': 'Buttons',
             'value_when_pressed': True,
             'pull': 'UP',
             'pins':
                 {'message0': 'GP0',
                  'message1': 'GP1',
                  'message2': 'GP2'}
        }
    }