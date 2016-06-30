                                        #Simple EFI Persistent Counter

#NEED A TEENSY
#NEED 2 Computers
#NEED Arduino IDE


Extending the work done by Ovrtech by adding a non volatile counter so can figure the key out without needing a timer.

#First load the sketch efi_booter_cracker.ino into the teensy 3.2 device.
Then run the device on your Macintosh device, I tested on 2 MacBookPro Device ranging from El Capitan and Mountain Lion.
After the password is correctly guessed by the teensy, !!!please take out the power!!! Iterations is how the teensy is set, so if no power no iterations hence the persisten counter will be haulted.


#Second upload the iteration_read.ino file to the teensy.
Now observe through Arduino Serial Montior for memory adress 20 and the iteration count
for eaxample if the value is something like 20 2 , it is suppose to indicate 0001 as the pin.
