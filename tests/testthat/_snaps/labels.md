# Labelling dataframes

    Code
      get_label(xx)
    Output
                          model                       mpg                       cyl 
                        "Model"       "Miles/(US) gallon"                     "cyl" 
                           disp                        hp                      drat 
        "Displacement (cu.in.)"        "Gross horsepower"         "Rear axle ratio" 
                             wt                      qsec                        vs 
            "Weight (1000 lbs)"           "1/4 mile time"                  "Engine" 
                             am                      gear                      carb 
                 "Transmission" "Number of forward gears"   "Number of carburetors" 
                        hp_date                qsec_posix 
           "Some nonsense date"               "Date+time" 

# Labelling nested lists (get)

    Code
      get_label(x)
    Output
                                                                                    
                             NA                        NA                        NA 
              iris.Sepal.Length          iris.Sepal.Width         iris.Petal.Length 
              "Length of Sepal"          "Width of Sepal"         "Length of Petal" 
               iris.Petal.Width              iris.Species                     model 
               "Width of Petal"                  "Specie"                   "Model" 
                            mpg                       cyl                      disp 
            "Miles/(US) gallon"     "Number of cylinders"   "Displacement (cu.in.)" 
                             hp                      drat                        wt 
             "Gross horsepower"         "Rear axle ratio"       "Weight (1000 lbs)" 
                           qsec                        vs                        am 
                "1/4 mile time"                  "Engine"            "Transmission" 
                           gear                      carb                   hp_date 
      "Number of forward gears"   "Number of carburetors"      "Some nonsense date" 
                     qsec_posix                       foo                      ffoo 
                    "Date+time"                     "foo"                    "ffoo" 

---

    Code
      get_label(x, simplify = FALSE)
    Output
      [[1]]
      [1] NA NA NA
      
      [[2]]
              iris.Sepal.Length          iris.Sepal.Width         iris.Petal.Length 
              "Length of Sepal"          "Width of Sepal"         "Length of Petal" 
               iris.Petal.Width              iris.Species                     model 
               "Width of Petal"                  "Specie"                   "Model" 
                            mpg                       cyl                      disp 
            "Miles/(US) gallon"     "Number of cylinders"   "Displacement (cu.in.)" 
                             hp                      drat                        wt 
             "Gross horsepower"         "Rear axle ratio"       "Weight (1000 lbs)" 
                           qsec                        vs                        am 
                "1/4 mile time"                  "Engine"            "Transmission" 
                           gear                      carb                   hp_date 
      "Number of forward gears"   "Number of carburetors"      "Some nonsense date" 
                     qsec_posix 
                    "Date+time" 
      
      [[3]]
         foo   ffoo 
       "foo" "ffoo" 
      

