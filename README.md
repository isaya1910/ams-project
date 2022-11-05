# ams-project


Lesson: 
  provideStartTime(): DateTime
  duration(): Duration
  matherial(): Matherial
  
Course:
  futureLessons(): List<Lesson>
  endedLessons(): List<Lesson>
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
  createCourse()
  acceptLessonSkip()
  declineLessonSkip()
  acceptCoursePause()
  declineCoursePause()
  rescheduleLesson()
