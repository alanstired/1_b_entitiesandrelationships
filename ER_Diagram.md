erDiagram
    Student ||--o{ Course : Enrolls In
    Course }o--|| Homework : Has
    Student ||--o{ Submission : Submits
    Homework ||--o{ Submission : Has
    Course {
        string CourseID
        string CourseName
        string Instructor
        date StartDate
        date EndDate
    }
    Student {
        string StudentID
        string Name
        string Email
    }
    Homework {
        string HomeworkID
        string Description
        date DueDate
        int TotalPoints
    }
    Submission {
        string SubmissionID
        date SubmissionDate
        string Content
        int Grade
        string Comments
    }
