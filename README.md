# ams-project


Lesson: 
  provideStartTime(): DateTime
  duration(): Duration
  
Course:
  futureLessons(): List<Lesson>
  endedLessons(): List<Lesson>
  skipeedLessons(): List<Lesson>
  nextLesson(): Lesson
  
  
Student:
  requestLessonSkip(lesson: Lesson)
  requestLessonReschedule(lesson: Lesson): Lesson
  requestCoursePause()
  bonus(): Bonus
  
Teacher: 
  markAttendence(student: Student)
  giveBonus(student: Student)

Admin: 
  createCourseForStudent()
  acceptLessonSkip()
  declineLessonSkip()
  acceptCoursePause()
  declineCoursePause()
  rescheduleLesson()
