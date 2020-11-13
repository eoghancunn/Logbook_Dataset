# Logbook_Dataset
A dataset of climbing logbook comments for active learning and text classification. Each entry is a comment associated with the ascent of a route. 
The text of the comment and some additional metadata are provided. A small number (304) of the comments are labelled to indicate if they contain 'beta' for the route. Additional comments have been manually labelled by human annotators. These include comments that were queried by an active learner to be used as training data and comments that were annotated to be used as unseen test data

### Schema
Column # | Column | Description 
--- | ------ | -----  
 0  | _id                    | Unique Id for comment 
 1  | climber_id             | Unique Id for climber (anonomised)
 2  | comment                | Comment text
 3  | date                   | Date of ascent
 4  | final_test             | Boolean identifying comments annotated to be used as test data
 5  | label                  | Boolean indicating if the comment contains beta
 6  | local_to               | The climbing area that the climber is local to 
 7  | location               | The location of the route 
 8  | queried                | Boolean identifying comments queried for annotation
 9  | route_grade            | The grade of the route mapped to an interger for comparison
 10 | route_info             | The name and grade of the route 
 11 | unseen_test            | Boolean identifying comments annotated to be used as test data
 12 | max_grade_of_climber   | The max grade (as an integer) achieved by the climber in the year of the ascent 
 13 | challenge              | max_grade_of_climber - route_grade
 14 | is_local               | Boolean indicating if the climber was local to the area 
 15 | comment_len            | Character count of the comment
 16 | annotation             | Boolean label indicating if the comment contains beta - aggregated from 10 annotators 
