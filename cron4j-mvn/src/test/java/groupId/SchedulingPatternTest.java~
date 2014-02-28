package it.sauronsoftware;

import it.sauronsoftware.cron4j.SchedulingPattern;
import it.sauronsoftware.cron4j.InvalidPatternException;

import junit.framework.Test;
import junit.framework.TestCase;
import junit.framework.TestSuite;

public class SchedulingPatternTest extends TestCase{

  public static void testSetup() {
  }

  public static void testCleanup() {
    // Teardown for data used by the unit tests
  }

  public void testExceptionIsThrown() {
  	try{
   	 SchedulingPattern sp = new SchedulingPattern("0 5 * *");
   	}
   	catch(InvalidPatternException e){
   		assertTrue(true);
   	}
  }

  public void testPattern() {
    String pattern;
    pattern="0 5 * * *|8 10 * * *|22 17 * * *";
    assertTrue(pattern + " is correct", SchedulingPattern.validate(pattern));
    pattern="0 \t5 \t* \t* \t* \t";
    assertTrue(pattern + " is correct", SchedulingPattern.validate(pattern));
  }
}
