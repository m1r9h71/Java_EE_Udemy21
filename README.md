# Jave_EE_Udemy21
Differences between Stateful and Stateless EJBs
#This tutorial demonstates the difference between a Stateless and Stateful EJB
I created:
  @EJB(beanName = "flightStateless")
	private FlightLocal_ejb8 fs;
	
	@EJB(beanName = "flightStateless")
	private FlightLocal_ejb8 fs2;
	
	@EJB(beanName = "flightStateful")
	private FlightLocal_ejb8 fsStateful;
	
	@EJB(beanName = "flightStateful")
	private FlightLocal_ejb8 fsStateful2;
  
  and added a new setTo() and setFrom() for the stateful and the stateless objects.
  The Stateless object fs printout changed but the Stateful object fsStateful did not
  showing that the stateful object needs to be called directly to change whereas the stateless will create a new object each time.
  
