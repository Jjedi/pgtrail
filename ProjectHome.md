## A generic implementation of postgres audit trail from version 9 and higher ##

List of features:
  * Implemented purely in plpgsql. No need to install additional languages on database server. No need to compile/install modules
  * Single table log file. No need to create log table for individual table.
  * One log config table: Set the name of the schema and table, you are all set.
  * Lightweight. no information schema lookup during actual DML query.
  * No complicated dependency. Only a single contrib module(hstore)is used which is distributed on standard postgres distribution.