# Skill Schema

A set of schema classes for describing skills, experience and qualifications

This is a **DRAFT** of a proposed extension we intend to submit to schema.org.

## Purpose

Schema.org has filled out very nicely over the years and covers many use cases.
However it leaves areas underdeveloped.

For example the [JobPosting class](http://schema.org/JobPosting) defines a
skills property that accepts Text values. We feel that it would be useful to
define a Skill class that can be used to describe a skill and some properties
that could assist understanding of the attainment and development of that skill.

For the purposes of this proposal skill is defined as follows:

> Learned abilities to carry out specific tasks or apply specific domain knowledge

Skills exist in a topology, they may have dependencies (either soft or hard) 
and they may be related to or complemented by other skills. It is outside the
scope of this proposal to create a classification of skills but is intended
that the schema must be usable by future classifiers. It therefore desirable
to describe sufficient properties and structure to provide for this.

## How does this fit in with schema.org?

Various existing schema.org classes define properties for which our extended
schema might provide extended semantics.

[JobPosting](http://schema.org/JobPosting) defines the following properties:
	* experienceRequirements
	* qualifications
	* skills
	
[Profession](http://schema.org/Profession), a [proposed new class in core](https://www.w3.org/2015/11/06-schemed-minutes.html).
	
It has [been](https://github.com/schemaorg/schemaorg/issues/789 
[proposed](https://github.com/schemaorg/schemaorg/issues/807#issuecomment-144746086)
that [Person](http://schema.org/Person) should be extended with
[singular](https://www.w3.org/wiki/WebSchemas/Singularity) skill and
qualification properties. We feel this would be very useful and that our
propsed Skill, Experience and Qualification classes would provide extended
semantics for the aforementioned properties.
