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
  requestLessonSkip(course: Course, )
  requestLessonReschedule()
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
