# DavaBahti
This repo was created for final exam for "Software Design Patterns"

VM options:
--module-path "path to library" --add-modules javafx.controls,javafx.fxml

**
Need to download javafx javafx-sdk-25.0.1**


SQL:
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    username VARCHAR(50) UNIQUE NOT NULL,
    password VARCHAR(100) NOT NULL
);

CREATE TABLE vocabulary_questions (
    id SERIAL PRIMARY KEY,
    word TEXT NOT NULL,
    image_path TEXT NOT NULL,
    option1 TEXT NOT NULL,
    option2 TEXT NOT NULL,
    option3 TEXT NOT NULL,
    option4 TEXT NOT NULL,
    correct_answer TEXT NOT NULL
);

CREATE TABLE grammar_questions (
    id SERIAL PRIMARY KEY,
    question_text TEXT NOT NULL,
    option1 TEXT NOT NULL,
    option2 TEXT NOT NULL,
    option3 TEXT NOT NULL,
    option4 TEXT NOT NULL,
    correct_answer TEXT NOT NULL
);



INSERT INTO vocabulary_questions (word, image_path, option1, option2, option3, option4, correct_answer)
VALUES
    ('Astronaut', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\astronaut.png', 'Astronaut', '', 'Doctor', 'Engineer', 'Teacher', 'Astronaut'),
    ('Car', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\car.png', 'Bike', 'Plain', 'Car', 'Helicoptor', 'Car'),
    ('Money', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\money.png', 'Document', 'Money', 'Coin', 'ID cart', 'Money'),
    ('Dog', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\dog.png', 'Snake', 'Dog', 'Snail', 'Cat', 'Dog'),
    ('Door', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\door.png', 'Bed', 'Desk', 'Window', 'Door', 'Door'),
    ('Apple', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\apple.png', 'Apple', 'Banana', 'Orange', 'Grapes', 'Apple'),
    ('Book', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\book.png', 'Copybook', 'Notebook', 'Magazine', 'Book', 'Book'),
    ('House', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\house.png', 'House', 'Museum', 'Bank', 'Police Station', 'House'),
    ('Laptop', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\laptop.png', 'Phone', 'Laptop', 'Gloshka', 'Tablet', 'Laptop'),
    ('Sun', 'C:\\Users\\ryshy\\IdeaProjects\\DavaBahti\\src\\main\\images\\lsun.png', 'Moon', 'Air', 'Clouds', 'Sun', 'Sun'),

INSERT INTO grammar_questions (question_text, option1, option2, option3, option4, correct_answer)
VALUES
    ('The cat ___ on the mat.', 'sat', 'sits', 'sitting', 'is sitting', 'sat'),
    ('She ___ a book now.', 'read', 'reads', 'is reading', 'reading', 'is reading'),
    ('We ___ to the park tomorrow.', 'go', 'went', 'going', 'will go', 'will go'),
    ('I ___ a good student.', 'am', 'is', 'are', 'was', 'am'),
    ('He ___ to school by bus.', 'go', 'going', 'goes', 'is going', 'goes'),
    ('___ you like coffee?', 'Do', 'Does', 'Are', 'Is', 'Do'),
    ('She ___ her homework in the evening.', 'do', 'does', 'is doing', 'did', 'does'),
    ('They ___ to play football every weekend.', 'like', 'likes', 'are liking', 'liked', 'like'),
    ('My father ___ a doctor.', 'is', 'are', 'am', 'was', 'is'),
    ('We ___ friends for many years.', 'are', 'were', 'have been', 'had been', 'have been');


    
