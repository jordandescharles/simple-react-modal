# simple-react-modal
 
A simple Modal

Hi thanks for reading this, im Jordan and junior front dev. this is my first package, it's simple maybe a little bit messy, but a little achievement >

I DO NOT recommend you to use it hahahaha

This Component has been created for my OpenclassRooms project witch is not perfect,I may update it later to fix some bug and to reduce the sizes and files, this one was compiled with TSDX

CSS

base css you can include to your project to style the modal, you can also use some props to override some style if needed list below

.modal-container {
    display:none; 
    position: fixed; 
    width: 100%; 
    height: 100%;
    left: 0;
    top:0;
    background-color: #ffffffae;
    z-index: 1;
  }
.modal{
    background-color: black;
    color:White;
    border-radius: 10px;
    border: 1px solid black;
}
.modal p{
    margin-top: 30px;
}
.modalBtn{
    display: none;
    border: none;
    border-radius: 3px;
    padding: 5px;
    cursor: pointer;
}
.close{
   display: block;
   background-color: black;
   border-radius: 20px;
   width: 20px;
   height: 20px;
   float: right;
   transform: translateX(10px) translateY(-10px);
   cursor: pointer;
}

Usable PROPS

text: string display:string width:string height:string bgColor:string margin:string button:string buttonText:string buttonWidth:string buttonHeight: string buttonBgColor: string buttonBorder: string buttonMargin: string buttonPadding:string
How to use

Best way to trigger on/off the modal is to use Custom hook

const [displayModal, setdisplayModal] = useState(false)
< Modal display={displayModal} />

then on your submit button you can

 setdisplayModal(true)

don't forget to reset the state if you can use it more than once :
