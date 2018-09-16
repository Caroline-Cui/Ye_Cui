# Ye_Cui
//
//  ViewController.swift
//  CarolineApp
//
//  Created by 崔晔 on 9/10/18.
//  Copyright © 2018 崔晔. All rights reserved.
//

import UIKit

class ViewController: UIViewController {
    
    
    
    @IBOutlet weak var textField: UITextField!
    @IBOutlet weak var textLable: UILabel!
    
    
    var backgroundColor : UIColor!
    
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
        
        backgroundColor =
            view.backgroundColor
    }

    
    
    
    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

    
    @IBAction func dodTapButton(_ sender:Any){
        print("Hello")
        textLable.textColor = UIColor.orange
}

    
    @IBAction func didTapViewButton(_ sender: Any) {
        
        view.backgroundColor = UIColor.red
    }
 
    
    @IBAction func didTapTextButton(_ sender: Any) {
        textLable.text = textField.text
        textField.text = ""
        view.endEditing(true)
    }
    
    @IBAction func onResetGesture(_ sender: Any) {
        textLable.text = "Hello"
        view.backgroundColor =
        backgroundColor
        
    }
    
}
