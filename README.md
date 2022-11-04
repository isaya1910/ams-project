# ams-project


Lesson: 
  provideStartTime(): DateTime
  
Course:
  provideFutureLessons(): List<Lesson>
  providePreviousLessons(): List<Lesson>
  provideSkippedLessons(): Lesson
  skipLesson(lesson: Lesson)
  rescheduleLesson(lesson: Lesson): Lesson
  
  
  
Student:
  requestLessonSkip(lesson: Lesson)
  requestLessonReschedule(lesson: Lesson): Lesson
  requestCoursePause()
  provideBonus(): Bonus
  
Teacher: 
  markAttendence(student: Student)
  giveBonus(student: Student)

Admin: 
  acceptLessonSkip()
  declineLessonSkip()
  acceptCoursePause()
  declineCoursePause()
  rescheduleLesson()
