# ams-project


Lesson: 
  provideStartTime(): DateTime
  
Course:
  provideFutureLessons(): List<Lesson>
  providePreviousLessons(): List<Lesson>
  provideSkippedLesson(): Lesson
  
  
Student:
  requestLessonSkip(lesson: Lesson)
  requestLessonReschedule()
  requestCoursePause()
  provideBonus(): Bonus
  
Teacher: 
  markAttendence(student: Student)
  giveBonus(student: Student)

Admin: 
  acceptLessonSkip(lesson: Lesson)
  declineLessonSkip(lesson: Lesson)
  acceptCoursePause(course: Course)
  declineCoursePause(course: Course)
  rescheduleLesson(lesson: Lesson)
