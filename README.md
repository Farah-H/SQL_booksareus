# Specifications

1. We should have Users who have:
- email
- phone number
- name

2. E-Books:
- title
- location
- release date
- user who created it

3. We should be able to make a booking of an ebook:
- what ebook
- who rented out
- what date
- price

## Questions
- What is the relationship between the tables?
Please see png file, really depends on how the backend works.
- Who belongs to whom?
I don't understand this question... 
- Can user rent out books?
Yes. 
- how many 1:N relationships are there?
3
- Do we have or do we need a N:N relationship?
We can have one, if we allow bookings to have multiple books, but in this case I made the assumption that bookings with multiple books would be split into smaller transactions with one book each. It is possible to have a linking table to allow for a booking to have multiple tables, to avoid a many-to-many relationship. generally you want to avoid many-many relationships, hence the linking key or assumption for one-book transactions. 