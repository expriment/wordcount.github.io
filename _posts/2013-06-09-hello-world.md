---
layout: post
title: hello world
category: pandoc
---
hello

$e^x = \sum_{n=0}^\infty \frac{x^n}{n!} = \lim_{n\rightarrow\infty} (1+x/n)^n$

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ {.python .numberLines}
class FSM(object):

"""This is a Finite State Machine (FSM).
"""

def __init__(self, initial_state, memory=None):

    """This creates the FSM. You set the initial state here. The "memory"
    attribute is any object that you want to pass along to the action
    functions. It is not used by the FSM. For parsing you would
    typically pass a list to be used as a stack. """

    # Map (input_symbol, current_state) --> (action, next_state).
    self.state_transitions = {}
    # Map (current_state) --> (action, next_state).
    self.state_transitions_any = {}
    self.default_transition = None
    ...
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
