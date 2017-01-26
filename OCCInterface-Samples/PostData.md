### Create and control resources

Create the mindstorm : %{
  "text": "create-mindstorm",
  "put":
  [
    {
        "address": "/lego_mindstom_ntx2",
        "data": {
          "id": "urn:uuid:d99486b7-0632-482d-a184-a9195733ddd4",
		  "title": "robot vehicule claptap",
		  "summary": "First robot claptap story",
		  "kind": "http://occiware.org/lego_mindstorm#lego_mindstom_ntx2",
		  "attributes": {
			"name" : "ClapTrap",
			"mac_address" : "00:16:53:10:10:C3"
		  }
        }     
    }
  ]
}%

* %{
    "text": "↑forward",
    "post": {
      "address": "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4?action=move_forward",
      "data": {
        "action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#move_forward"
      }
    }
  }%
  
* %{
	"text": "↓backward",
	"post": {
	  "address": "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4?action=move_backward",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#move_backward"
	  }
	}
}%

* %{
	"text": "←left",
	"post": {
	  "address": "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4?action=rotate_left",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#rotate_left"
	  }
	}
}%

* %{
	"text": "→right",
	"post": {
	  "address": "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4?action=rotate_right",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#rotate_right"
	  }
	}
}%

* %{
	"text": "stop",
	"post": {
	  "address": "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4?action=stop_move",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#stop_move"
	  }
	}
}%


Create the robogator : %{
  "text": "create-robogator",
  "put":
  [
    {
        "address": "/robotgator",
        "data": {
		  "id": "urn:uuid:d99486b7-0632-482d-a184-a9195733ddd3",
		  "title": "robot gator 1",
		  "summary": "First robot gator story",
		  "kind": "http://occiware.org/lego_mindstorm#robotgator",
		  "attributes": {
			"name" : "Robogator",
			"mac_address" : "00:16:53:13:1B:B0"
		  }
        }     
    }
  ]
}%

* %{
    "text": "↑forward",
    "post": {
      "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=move_forward",
      "data": {
        "action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#move_forward"
      }
    }
  }%
  
* %{
	"text": "↓backward",
	"post": {
	  "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=move_backward",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#move_backward"
	  }
	}
}%

* %{
	"text": "←left",
	"post": {
	  "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3??action=rotate_left",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#rotate_left"
	  }
	}
}%

* %{
	"text": "→right",
	"post": {
	  "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3??action=rotate_right",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#rotate_right"
	  }
	}
}%

* %{
	"text": "stop",
	"post": {
	  "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=stop_move",
	  "data": {
		"action": "http://occiware.org/lego_mindstorm/lego_mindstom_ntx2/action#stop_move"
	  }
	}
}%

* %{
    "text": "open_mouth",
    "post": {
      "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=open_mouth",
      "data": {
        "action": "http://occiware.org/lego_mindstorm/robotgator/action#open_mouth"
      }
    }
  }%

* %{
    "text": "close_mouth",
    "post": {
      "address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=close_mouth",
      "data": {
        "action": "http://occiware.org/lego_mindstorm/robotgator/action#close_mouth"
      }
    }
  }%
  
* %{
	"text": "read_ultra_sound",
		"post": {
			"address": "/robotgator/d99486b7-0632-482d-a184-a9195733ddd3?action=read_ultra_sound",
			"data": {
				"action": "http://occiware.org/lego_mindstorm/robotgator/action#read_ultra_sound"
			}
		}
	}%
	
	
Create the Turtlebot : %{
  "text": "create-turtlebot",
  "put":
  [
    {
        "address": "/turtlebot",
        "data": {
          "id": "urn:uuid:d99486b7-0632-482d-a184-a9195733ddd5",
		  "title": "robot vehicule turtlebot",
		  "summary": "First turtlebot story",
		  "kind": "http://occiware.org/turtlebot#turtlebot",
		  "attributes": {
			"user" : "turtlebot",
			"ip_address" : "192.168.137.212",
			"password" : "turtlebot"
		  }
        }     
    }
  ]
}%

* %{
    "text": "↑forward",
    "post": {
      "address": "/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5?action=move_forward",
      "data": {
        "action": "http://occiware.org/turtlebot/turtlebot/action#move_forward"
      }
    }
  }%
  
* %{
	"text": "↓backward",
	"post": {
	  "address": "/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5?action=move_backward",
	  "data": {
		"action": "http://occiware.org/turtlebot/turtlebot/action#move_backward"
	  }
	}
}%

* %{
	"text": "←turn left",
	"post": {
	  "address": "/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5?action=turn_left",
	  "data": {
		"action": "http://occiware.org/turtlebot/turtlebot/action#turn_left"
	  }
	}
}%

* %{
	"text": "→turn right",
	"post": {
	  "address": "/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5?action=turn_right",
	  "data": {
		"action": "http://occiware.org/turtlebot/turtlebot/action#turn_right"
	  }
	}
}%

* %{
	"text": "stop",
	"post": {
	  "address": "/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5?action=stop",
	  "data": {
		"action": "http://occiware.org/turtlebot/turtlebot2/action#stop"
	  }
	}
}%
  
 

Finally, you can delete the ressource you posted by clicking %{
  "text": "here",
  "del": [
    "/lego_mindstom_ntx2/d99486b7-0632-482d-a184-a9195733ddd4",
	"/robotgator/d99486b7-0632-482d-a184-a9195733ddd3",
	"/turtlebot/d99486b7-0632-482d-a184-a9195733ddd5"
  ]
}%
