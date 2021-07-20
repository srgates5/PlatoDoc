Plato Input Deck
================

.. _introduction:

Introduction
------------

This describes the Plato input deck. The Plato input deck contains the “recipe”for running a Plato optimization problem. A Plato problem is either a topology optimiza-tion problem or a shape/CAD parameter optimization problem.  In these problems we aretrying to optimize the toplogy or CAD parameters such that the resulting design meetssome  user-defined  perfromance  objective.   These  types  of  problems  require  a  geometricdefinition of the design domain as well as instructions about what the objectives and con-straints are,  what physics codes will be used to evaluate the objectives and constraints,what optimization algorithm to use, and variuos other parameters.  The geoemtry is gen-erally provided in the form of a finite element mesh and all of the other instructions arecontained in the Plato input deck.  This document will define general concepts used in thesetup of a Plato optimization problem and will then define all of the possible options thatcan be included in the input deck.

.. _general concepts:

General Concepts
----------------

Optimization problems can be very complex and require lots of different information.  ThePlato  input  deck  is  designed  to  be  very  general  in  the  way  it  defines  an  optimizationproblem breaking it down into its fundamental pieces that can be combined in differentways to define different kinds of problems.  There are 5 main building blocks upon whichall optimziation problems are defined in Plato.  This section will briefly introduce thesebuilding blocks and describe how they are used to define an optimization problem.
