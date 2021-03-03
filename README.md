db.books.insertMany([
    {
      title: "Up, down",
      description: "awesome books",
      authors: "John Google"
    },
    {
      title: "Left, right",
      description: "super",
      authors: "Alex Ya"
    },
]);

db.books.find({title: 1});

db.books.updateOne({ _id: req.params.id }, {$set: {description: req.body.description, authors: req.body.authors }})