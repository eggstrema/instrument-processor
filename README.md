# Instrument Processor

Java version for the Instrument Processor Kata by Urs Enzler:
https://www.planetgeek.ch/2010/03/28/mocking-kata-instrument-processor-net/

## Your Task
The exercise is to implement the `InstrumentProcessor` in a way that:
* When the method `process()` is called then the `InstrumentProcessor` gets the
  next task from the `TaskDispatcher` and executes it on the `Instrument`.
* When the `execute()` method of the `Instrument` throws an exception then this
  exception is passed on to the caller of the `process()` method.
* When the instrument runs the `eventHandlerFinished` then the `InstrumentProcessor`
  calls the task dispatcher’s `finishedTask()` method with the correct task.
* When the `Instrument` runs the `eventHandlerError` then the `InstrumentProcessor`
  writes the string  'Error occurred' to the console.
