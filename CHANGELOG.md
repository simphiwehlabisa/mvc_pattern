## 3.4.1
 Apr. 12, 2019
- Return _rebuildAllowed = true; in didUpdateWidget() & reassemble()

## 3.4.0
 Apr. 09, 2019
- Only dispose a Controller if no longer relied on by a view.

## 3.3.4
 Apr. 03, 2019
- **Correction** Controllers and Listeners dispose calls in the StateMVC were not an issue after all.

## 3.3.3
 Apr. 02, 2019
- Call _disposeState() on all controllers when StateMVC is disposed.

## 3.3.2
 Apr. 02, 2019
- Proven prudent to not dispose any Controllers or Listeners in the StateMVC.
 
## 3.3.1
 Apr. 02, 2019
- ControllerMVC getter 'states' returns a 'copy' of the Set of State objects. 
- Only dispose a Controller if no longer relied on by a view.

## 3.3.0 
 Mar. 16, 2019. 
- Removed abstract from class ControllerMVC
- Add didPopRoute() didPushRoute() to StateListener

## 3.2.4 
 Mar. 02, 2019. 
- No 'setState()' function is necessary; in some events.

## 3.2.3 
 Feb. 20, 2019. 
- await (con as AppConMVC)?.init();

## 3.2.2 
 Feb. 17, 2019. 
- _oldOnError = _recOnError()

## 3.2.1 
 Feb. 06, 2019. 
- Update the upper bound of the SDK constraint to <3.0.0

## 3.2.0 
 Jan. 30, 2019. 
- Deprecated Error Handler from Controller. Removed refresh(); from initState() & deactiveate

## 3.1.0 
 Jan. 26, 2019. 
- StateViewMVC implements StateListener & get controller 
 
## 3.0.0 
 Jan. 25, 2019. 
- Changed class StateListener to a mixin
- addState() in Controller and Listener adding any number of Views
- abstract class StateViewMVC<T extends StatefulWidget> extends StateMVC<T>
- class ViewMVC extends _StateObserver with _ControllerListing 
- void didChangeDependencies() will not refresh() on first build
- Removed from Controllers the getters: widget, context, mounted
- stateView getter is deprecated. Replaced by stateMVC. Removed stateMVC setter.
- Removed controller setter in class ViewMVC
- if (con is AppConMVC) //bool addBeforeListener(StateListener listener)

## 2.0.2 
 Jan. 19, 2019. 
- void addState(StateMVC state) {

## 2.0.1 
 Jan. 16, 2019. 
- AppMVC({this.con, Key key}) : super(key: key);

## 2.0.0 
 Jan. 16, 2019.   
- ControllerMVC(State state)
- class _StateView with StateListener
- _StateView() : _oldOnError = _recOnError() {
- abstract class StateMVC<T extends StatefulWidget> extends State<StatefulWidget>
- remove setter, controller
- _StateListener.disposeStateEventList() use clear();
- Removed StatefulWidgetMVC
- Removed StatedWidget
- abstract class AppMVC extends StatefulWidget {
- Removed StatelessWidgetMVC

## 1.3.6 
 Jan. 12, 2019.   
- StateListener to replace StateEvents. addState() disposedState()

## 1.3.5 
 Jan. 11, 2019.   
- remove StateListener

## 1.3.4 
 Jan. 11, 2019.   
- StateListener as a mixin for StateEvents

## 1.3.3 
 Jan. 01, 2019.   
- Removed @protected from ViewMVC.build()  Private _ControllerListing._con(String keyId)


## 1.3.2 
 Dec. 28, 2018.   
- if(mounted) in refresh()

## 1.3.1 
 Dec. 10, 2018.   
- sdk: ">=2.0.0 <5.0.0"

## 1.3.0 
 Dec. 03, 2018.   
- Updated README.md

## 1.3.0 
 Nov. 18, 2018.   
- add some further examples under test folder

## 1.2.4 
 Nov. 17, 2018.   
- fix on StateEvents assign on keyId

## 1.2.3 
 Nov. 13, 2018.   
- test for TestWidgetsFlutterBinding

## 1.2.2 
 Nov. 02, 2018.   
- fix on StatedWidget

## 1.2.1 
 Nov. 02, 2018.   
- fix on StateViewMVC

## 1.2.0 
 Oct. 29, 2018.   
- enhance AppMVC

## 1.1.1 
 Oct. 27, 2018.   
- StatefulWidgetMVC deemed deprecated

## 1.1.0 
 Oct. 25, 2018.   
- keyId in StateEvents

## 1.0.0 
 Oct. 24, 2018.   
- Official Production Release

## 0.0.14 
 Oct. 24, 2018.   
- fix on StateViewMVC & AppMVC & @protected

## 0.0.13 
 Oct. 23, 2018.   
- fix on _ControllerListing

## 0.0.12 
 Oct. 23, 2018.   
- class ViewMVC with _ControllerListing

## 0.0.11 
 Oct. 23, 2018.   
- class StateMVC with _ControllerListing, _StateEventList

## 0.0.10 
 Oct. 22, 2018.   
- include travis.yml

## 0.0.9 
 Oct. 21, 2018.   
- fix on ViewMVC & StateViewMVC

## 0.0.8 
 Oct. 20, 2018.   
- Updated the README.md

## 0.0.7 
 Oct. 19, 2018.   
- Provide example/main.dart

## 0.0.6 
 Oct. 18, 2018.   
- fix on StateMVC.con()

## 0.0.5 
 Oct. 18, 2018.   
- fix on StatedWidget

## 0.0.4 
 Oct. 18, 2018.   
- fix on StateMVC.add()

## 0.0.3 
 Oct. 18, 2018.  
- fix on AppMVC and StateEvents

## 0.0.1 
 Oct. 13, 2018. 
- Initial Release