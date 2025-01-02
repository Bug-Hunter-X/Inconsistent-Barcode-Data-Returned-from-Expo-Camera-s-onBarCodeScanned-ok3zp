# Inconsistent Barcode Data from Expo Camera's onBarCodeScanned

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` prop inconsistently returns barcode data.  Despite a successful scan, the function sometimes returns null or an incomplete result.  This is especially problematic when reliability is crucial.  The `bug.js` file showcases the problem, while `bugSolution.js` presents a potential workaround (though not a perfect solution). 

## Reproducing the Bug

1. Clone this repository.
2. Install dependencies: `npm install` or `yarn install`.
3. Run the app: `expo start`.
4. Attempt to scan various barcodes.  Observe instances where no data or incorrect data is returned.

## Potential Solutions (Workarounds)

The proposed solution involves adding error handling and retry mechanisms, along with careful checks of the returned data structure. However, a more robust and reliable solution would ideally be implemented within the Expo Camera API itself. Please report this issue to Expo directly for a more permanent fix.