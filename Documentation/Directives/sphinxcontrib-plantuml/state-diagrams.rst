.. include:: /Includes.rst.txt
.. index:: plantuml; state diagram
.. _Plantuml-state-diagrams:

===========================
Plantuml state diagrams
===========================

Taken from: https://plantuml.com/state-diagram


State diagram - Composite state
===============================

.. uml::

   [*] --> NotShooting

   state NotShooting {
     [*] --> Idle
     Idle --> Configuring : EvConfig
     Configuring --> Idle : EvConfig
   }

   state Configuring {
     [*] --> NewValueSelection
     NewValueSelection --> NewValuePreview : EvNewValue
     NewValuePreview --> NewValueSelection : EvNewValueRejected
     NewValuePreview --> NewValueSelection : EvNewValueSaved

     state NewValuePreview {
        State1 -> State2
     }

   }


State diagram - Fork
====================

.. uml::

   state fork_state <<fork>>
   [*] --> fork_state
   fork_state --> State2
   fork_state --> State3

   state join_state <<join>>
   State2 --> join_state
   State3 --> join_state
   join_state --> State4
   State4 --> [*]


State diagram - Conditional
===========================

.. uml::

   state "Req(Id)" as ReqId <<sdlreceive>>
   state "Minor(Id)" as MinorId
   state "Major(Id)" as MajorId

   state c <<choice>>

   Idle --> ReqId
   ReqId --> c
   c --> MinorId : [Id <= 10]
   c --> MajorId : [Id > 10]


State diagram - Note
====================

.. uml::

   [*] --> Active
   Active --> Inactive

   note left of Active : this is a short\nnote

   note right of Inactive
     A note can also
     be defined on
     several lines
   end note
