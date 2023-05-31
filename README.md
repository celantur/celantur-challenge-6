Data modelling Proof-of-Concept
================================

This challenge serves as the basis for the technical interview.

**Before starting the challenge**, please have a look at the challenge and tell us 
- if any aspect is unclear to you,
- if you want to amend the challenge to better reflect your skills,
- if you want to change / reduce the scope to better fit your time schedule,
- how much effort in your estimate you will need to finish it, and
- when you can finish the task.

We understand that you have other priorities and can not commit full time to completing the challenge.
Thus spend your time economically:
- You don't need to waste time on debugging. If it doesn't work, leave it.
- If anything is unclear, write us instead of guessing what we expect. 
- You don't need to learn a new technology. We can adapt the challenge 
  so that you can solve it with what you already know.

Don't hesitate to write us if you have any questions during the challenge.


Description
-----------

We have a scalable anonymisation solution with following layers:

- REST API: User uses the REST API to upload images or videos, query the status of the files (new, processing, processed, deleted) and download the anonymised files.
- Storage: Binary files are stored in S3 and processing information (upload-time, processing-time, number of anonymised objects etc) are stored in a NoSQL database.
- Processor: Files are processed via stateless processing instances. The instances need to know what objects (face, person, license plate, vehicle) need to anonymised 
  for each image or video.


Tasks
-----

### Coding challenge

- Create entity-relationship diagrammes for the database.
- Implement data models for the processor, storage and REST layers using `dataclasses` or Pydantic.
- Share your (private) repository with [@celantor](https://github.com/celantor).


### Pre-interview preparations

- Reflect on your last major software project. 
  What were the customer requirements? 
  What were the (technical and non-technical) challenges? 
- Fill out the [Self-evaluation matrix](./Self-Evaluation.md).


Deliverables
------------

- [ ] Code and diagrammes.
- [ ] Documentation how to run the code.
- [ ] [Self-evaluation matrix](./Self-Evaluation.md).
