public void paint(Graphics g)
	{
   
      int width = 980;
      int height = 630;
         
      g.drawRect( 10 , 10 , width , height );
//============================//        
    // Draw bottom-right //
//----------------------------//
      
      int xInitial = 10;
      int yInitial = 10;
      int pRate = 0;

      for (int qVCL = 0 ; qVCL <= 630 ; qVCL += 13 )
      {
      
         g.setColor( randomColor() );
      
         g.drawLine( xInitial + pRate , height + yInitial , width + xInitial , ( height + yInitial ) - qVCL );
         pRate += 20;
         
       }
//===========================//         
    // Draw bottom-left //
//---------------------------//
      
      xInitial = 10;
      yInitial = 10;
      pRate = 0;
      
      for (int qVCL = 0 ; qVCL <= 630 ; qVCL += 13 )
      {
      
         g.setColor( randomColor() );
      
         g.drawLine( xInitial + pRate , height + yInitial , 0 + xInitial , ( 0 + yInitial ) + qVCL );
         pRate += 20;
         
      }
//========================//    
    // Draw top-left //
//------------------------//
      
      xInitial = 10;
      yInitial = 10;
      pRate = 0;
      
      for (int qVCL = 0 ; qVCL <= 630 ; qVCL += 13 )
      {
      
         g.setColor( randomColor() );
      
         g.drawLine( xInitial + pRate , 0 + yInitial , 0 + xInitial , ( height + yInitial ) - qVCL );
         pRate += 20;
         
      }
//========================//    
    // Draw top-right //
//------------------------//
      
      xInitial = 10;
      yInitial = 10;
      pRate = 0;
      
      for (int qVCL = 0 ; qVCL <= 630 ; qVCL += 13 )
      {
      
         g.setColor( randomColor() );
      
         g.drawLine( xInitial + pRate , 0 + yInitial , width + xInitial , ( 0 + yInitial ) + qVCL );
         pRate += 20;
         
      }
	}
}
