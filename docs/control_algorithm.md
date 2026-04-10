# Control Algorithm

Read front LDR  
Read back LDR  

difference = front − back

if abs(difference) < threshold
    stop motors

else if difference > threshold
    move forward

else
    move backward
